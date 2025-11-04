# Language Models

- [LLM / transformer slides](https://docs.google.com/presentation/d/1vjuH1YCsna0hk5VGpZ6H201B-LkBLvIYhgStTTEPpBc/edit?usp=sharing)

## Sequential Data and Recurrent Neural Networks

- 📚 [The Unreasonable Effectiveness of RNNs](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
- 🎨 [Four Experiments in Handwriting with a Neural Network](https://distill.pub/2016/handwriting/) (Drawing)
- 📖 [10 things artificial intelligence did in 2018](http://aiweirdness.com/post/181621835642/10-things-artificial-intelligence-did-in-2018) by Janelle Shane (Text)
- 📖 [Writing with the Machine](https://www.robinsloan.com/notes/writing-with-the-machine/)

## Transformers and Large Language Models

> among the reasons I use large pre-trained language models sparingly in my computer-generated poetry practice is that being able to know whose voices I'm speaking with is... actually important, as is being understanding how the output came to have its shape - [@aparrish](https://twitter.com/aparrish/), [full thread](https://twitter.com/aparrish/status/1286808606466244608)

- 📚 [Watch an A.I. Learn to Write by Reading Nothing but **\_\_\_\_**](https://www.nytimes.com/interactive/2023/04/26/upshot/gpt-from-scratch.html) by Aatish Bhatia
- 📚 [Attention is All You Need](https://arxiv.org/abs/1706.03762) - Original "Transformer" paper from 2017, also [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473) -- Attention paper from 2014
- 📚 [What Are Transformer Models and How Do They Work?](https://cohere.com/llmu/what-are-transformer-models)
- 🎥 [How large language models work, a visual intro to transformers](https://youtu.be/wjZofJX0v4M) by 3Blue1Brown
- 🎥 [Intro to Large Language Models](https://youtu.be/zjkBMFhNj_g) by Andrej Karpathy and [Intro to LLMs slides](https://drive.google.com/file/d/1pxx_ZI7O-Nwl7ZLNk5hI3WzAsTLwvNU7/view)
- 📖 [Language Models Can Only Write Ransom Notes](https://posts.decontextualize.com/language-models-ransom-notes/) by Allison Parrish

## Writing with LLMs

- **Jhave Johnston** – _ReRites_
  Human-AI poetic collaboration across a full poetry corpus.
  🔗 [https://glia.ca/rerites/](https://glia.ca/rerites/)

- **K. Allado-McDowell** – _Pharmako-AI_
  GPT-3 dialogue on ecology, nonhuman consciousness, and techno-poetics.
  🔗 [https://www.kalladomcdowell.com/pharmakoai](https://www.kalladomcdowell.com/pharmakoai)

## LLM Training

- 🦙 [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/pdf/2302.13971.pdf)
- 🦙 [The Llama 3 Herd of Models](https://arxiv.org/pdf/2407.21783)
- 🦜 [On the Dangers of Stochastic Parrots: Can Language Models Be Too Big? 🦜](https://dl.acm.org/doi/10.1145/3442188.3445922)
- 🔍 [The Foundation Model Transparency Index](https://crfm.stanford.edu/fmti/May-2024/index.html)
- 📖 [Generative AI’s Illusory Case for Fair Use](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4924997) by Jacqueline Charlesworth

### Datasets for LLMs

- 🔢 [Common Crawl](https://commoncrawl.org/)
- 🔢 [The Pile](https://pile.eleuther.ai/)
- 🔢 [FineWeb-Edu](https://huggingface.co/datasets/HuggingFaceFW/fineweb-edu)
- 🔢 [SmolLM Corpuse](https://huggingface.co/datasets/HuggingFaceTB/smollm-corpus)

### Climate Impact

- 🌏 [The Internet’s Next Great Power Suck](https://www.theatlantic.com/technology/archive/2023/08/ai-carbon-emissions-data-centers/675094/)
- ⚡️ [Carbon Emissions and Large Neural Network Training ](https://arxiv.org/ftp/arxiv/papers/2104/2104.10350.pdf)

## Web Servers with Node.js + p5.js

- 🎥 [Workflow: Terminal, Shell, Node.js, VSCode](https://thecodingtrain.com/tracks/discord-bots/discord/2023-workflow)
- 🎥 [How to Set Up a Node.js Project](https://thecodingtrain.com/tracks/discord-bots/discord/setup-node-project)
- 🎥 [Server Side / Express with node.js](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/1-server-side-with-node-js)
- 🎥 [HTTP "POST" request with fetch](https://thecodingtrain.com/tracks/data-and-apis-in-javascript/data/2-data-selfie-app/3-http-post-request)
- 💻 [Hello World node.js + express + p5 example](https://github.com/Programming-from-A-to-Z/Simple-Express-p5.js)

## Code Examples and Implementations

### Local LLM Models

- 🦙 [Ollama: Run LLMs locally](https://ollama.ai/)
- 📋 [Ollama API Docs](https://github.com/ollama/ollama/blob/main/docs/api.md)
- 💻 [Ollama with node.js and JavaScript](https://github.com/Programming-from-A-to-Z/Ollama-Examples)
- 💻 [LMStudio](https://lmstudio.ai/)

### Nanochat

- [nanochat](https://github.com/karpathy/nanochat)

### OpenAI API

- [OpenAI API Docs](https://platform.openai.com/docs/api-reference/introduction)
- [Ollama Code with OpenAI instead](https://github.com/Programming-from-A-to-Z/Ollama-Examples/tree/openai)

### Transformers.js

- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js/)
- [SmolLM 3](https://github.com/huggingface/smollm)
- 💻 [p5.js LLM examples](https://editor.p5js.org/a2zitp/collections/Y1oZ1As1s)

## Reasoning Models

Reasoning models are a type of large language model trained (or fine-tuned) to solve multi-step problems. They use "chain-of-thought" reasoning to plan, reflect, and revise their answers and generate “thoughts” before giving the final response. You can think of them as LLMs with an inner monologue.

- [Ollama "thinking" models](https://ollama.com/search?c=thinking)
- [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948)
- [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050)
- [What is a reasoning model?](https://www.ibm.com/think/topics/reasoning-model)

## Assignment

- Read [Dismantling the Empire of AI with Karen Hao](https://www.bloodinthemachine.com/p/dismantling-the-empire-of-ai-with) and [Karen Hao on how the AI boom became a new imperial frontier](https://www.reuters.com/lifestyle/karen-hao-how-ai-boom-became-new-imperial-frontier-2025-07-03/)
- Experiment with prompting a large language model in some way other than a provided interface (e.g. ChatGPT) and document the results in a blog post. Consider how working with an LLM compares to generating text from the other methods including but not limited to markov chains and context free grammars. In your blog post, reflect on how your experiment relates to themes from the readings—whether that's labor, environmental impact, data extraction, corporate narratives, or something else. Here are some options:
  - Run [any of the code examples above](#code-examples-and-implementations) Try adjusting the prompts, interaction, or visual design.
  - Try a variety of models locally with [Ollama](https://ollama.ai/) or [LMStudio](https://lmstudio.ai/). Compare and contrast different models.
  - Can you connect an LLM to a Discord Bot or other platform?
  - Invent your own idea! Think weird, critical, poetic, or subversive.

## Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- name [post title](url)
- Haya [Book recommender](https://www.notion.so/Book-recommender-29cc09edca1780af85f4ec67ef7a1e38?source=copy_link)
- Junqi [emotion analysis test](https://fuzzy-mask-71e.notion.site/COMPUTATIONAL-TEXT-A-Z-262480e9e232806f96c3f65ab685c294?source=copy_link)
- Olivia [oracle](https://www.notion.so/CompText-7-LLMs-Oracle-2a0d586d7a8d80eda08be0fbebc797bf?source=copy_link)
- Fiona Huang [Week 8 assignment experiment](https://www.notion.so/Week-8-Assignment-Experiment-2a0701873e078003891ae2e2911d47e4)