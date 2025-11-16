# MCP + LM Studio

## What is MCP?

**MCP (Model Context Protocol)** is an open standard for connecting LLM apps to external tools and data in a consistent way.

- MCP servers expose tools, resources, prompts, etc.
- MCP clients (LM Studio, Claude Desktop, VS Code, ChatGPT Desktop, etc.) connect to those servers and let the model call the tools.

### Resources

- [Model Context Protocol](https://modelcontextprotocol.io)
- [Introducing the Model Context Protocol](https://www.anthropic.com/news/model-context-protocol)
- [Claude Docs Overview](https://docs.claude.com/en/docs/mcp)

> Think of MCP like a USB-C port for AI applications. Just as USB-C provides a standardized way to connect your devices to various peripherals and accessories, MCP provides a standardized way to connect AI models to different data sources and tools.

## What is LM Studio?

**LM Studio** (similar to Ollama) is a desktop app that downloads and runs local LLMs. It can also act as an **MCP host**:

- You can plug in MCP servers (including ones you write yourself).
- The local model can then call those tools.

- [LM Studio](https://lmstudio.ai)
- [LM Studio MCP docs](https://lmstudio.ai/docs/app/mcp)

## How To

### Set up the MCP server with node.js

```bash
mkdir hello-mcp
cd hello-mcp
npm init -y
npm install @modelcontextprotocol/sdk express zod
```

Make sure `package.json` has `"type": "module"`:

```json
{
  "name": "mcp-hello-world",
  "version": "1.0.0",
  "type": "module",
  "main": "server.js",
  "scripts": {
    "start": "node server.js"
  },
  "dependencies": {
    "@modelcontextprotocol/sdk": "^1.22.0",
    "express": "^5.1.0"
  }
}
```

### Create `server.js`

```js
import express from 'express';
import { z } from 'zod';
import { McpServer } from '@modelcontextprotocol/sdk/server/mcp.js';
import { StreamableHTTPServerTransport } from '@modelcontextprotocol/sdk/server/streamableHttp.js';

const server = new McpServer({
  name: 'hello-mcp',
  version: '1.0.0',
});

server.registerTool(
  'say_hello',
  {
    title: 'Say Hello',
    description: 'Return a friendly greeting',
    inputSchema: { name: z.string() },
    outputSchema: { greeting: z.string() },
  },
  async ({ name }) => {
    console.log('say_hello called with name:', name);
    const greeting = `Hello, ${name}!`;

    return {
      content: [{ type: 'text', text: greeting }],
      structuredContent: { greeting },
    };
  }
);

const app = express();
app.use(express.json());

app.post('/mcp', async (req, res) => {
  const transport = new StreamableHTTPServerTransport({
    sessionIdGenerator: undefined,
    enableJsonResponse: true,
  });

  res.on('close', () => transport.close());

  await server.connect(transport);
  await transport.handleRequest(req, res, req.body);
});

const port = Number(process.env.PORT || 3000);
app.listen(port, () => {
  console.log(`MCP Hello server running on http://localhost:${port}/mcp`);
});
```

Then run:

```bash
npm start
```

You should see:

```text
MCP Hello server running on http://localhost:3000/mcp
```

The MCP server has one tool:

- `say_hello(name: string)`

### Configure MCP in LM Studio

LM Studio reads MCP config from an `mcp.json` file.

1. Download a model (let's use `openai/gpt-oss-20b`)
2. Go to a new chat and click the integrations plug --> Install --> edit `mcp.json`.
3. Add your local server:

```json
{
  "mcpServers": {
    "hello-mcp": {
      "url": "http://localhost:3000/mcp"
    }
  }
}
```

### Chat

In a new chat (with tools enabled), try:

```text
Call say_hello for {"name": "ITP Student"} and show me the result!
```

You can also try seeing if the model will intelligently call the tool on its own.

```text
Say hello to ITP student!
```

### Calling a Weather API

Register another tool

```js
server.registerTool(
  'get_weather',
  {
    title: 'Get Weather',
    description: 'Fetch current weather using the Open-Meteo API',
    inputSchema: {
      latitude: z.number(),
      longitude: z.number(),
    },
    outputSchema: {
      temperature: z.number(),
      precipitation: z.number(),
      humidity: z.number(),
    },
  },
  async ({ latitude, longitude }) => {
    const url = `https://api.open-meteo.com/v1/forecast?latitude=${latitude}&longitude=${longitude}&current=temperature_2m,precipitation,weather_code,relative_humidity_2m`;
    const response = await fetch(url);
    const data = await response.json();
    const current = data.current;
    const { temperature_2m, precipitation, relative_humidity_2m } = current;

    const summary = `Current temperature: ${temperature_2m}°C, precipitation: ${precipitation}mm, humidity: ${relative_humidity_2m}%`;

    console.log('get_weather called with', { latitude, longitude });
    console.log('get_weather result:', summary);

    return {
      content: [{ type: 'text', text: summary }],
      structuredContent: {
        temperature: temperature_2m,
        precipitation: precipitation,
        humidity: relative_humidity_2m,
      },
    };
  }
);
```

Now try:

```text
Call the "get_weather" tool with {"latitude": 40.7128, "longitude": -74.0060} and show me the result.
```

Or see if it can infer the right tool to call.

```text
Tell me the weather in New York City.
```

### Try another MCP Server like "Brave Web Search"

```json
{
  "mcpServers": {
    "hello-mcp": {
      "url": "http://localhost:3000/mcp"
    },
    "brave-search": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-brave-search"],
      "env": {
        "BRAVE_API_KEY": "API KEY HERE"
      }
    }
  }
}
```

```text
Call the "brave_web_search" tool with {"query": "p5.js creative coding", "count": 3} and summarize the top results.
```

```text
Search the web for "p5.js creative coding" summarize what you find!
```

### Also, jina.ai offers some options with a free API key

```json
    "jina-mcp-server": {
      "url": "https://mcp.jina.ai/sse",
      "headers": {
        "Authorization": "Bearer ${JINA_API_KEY}"
      }
    }
```

_(This belongs inside "mcpServers" merged with any existing entries.)_

For example, it can read a webpage.

```text
Please read https://natureofcode.com/ and summarize it.
```

## Testing with MCP Inspector

For debugging, you can also use the **MCP Inspector**

```bash
npx @modelcontextprotocol/inspector
```

## MCP servers can also connect to commercial LLM tools

- [Claude Desktop / Claude Code](https://docs.claude.com/en/docs/mcp)
- [VS Code with GitHub Copilot MCP servers](https://code.visualstudio.com/docs/copilot/customization/mcp-servers)
- [How to add Brave Search to Claude Desktop with MCP](https://brave.com/search/api/guides/use-with-claude-desktop-with-mcp)
