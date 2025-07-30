# 🛠️ ML Tools for Computational Text

**Supplement to the Computational Text from A to Z Resource Guide**
_Organized by the Equitable Syllabus Project_

This document organizes machine learning tools for working with text—grouped by access model, type, and intended usage. It’s designed to help students, artists, and researchers choose appropriate tools for creative, ethical, and exploratory projects.

---

## 🔓 Open Weight / Self-Hosted Models

These models can be downloaded and run locally, offering more transparency and experimentation potential.

| Tool/Model                                               | Description                                                                                   | Tags                                       |
| -------------------------------------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------ |
| **[Whisper](https://github.com/openai/whisper)**         | Open-source speech-to-text model by OpenAI. Great for transcription and voice-based projects. | `TTS/voice`, `open`, `offline`, `creative` |
| **[LLaMA](https://ai.meta.com/llama/)**                  | Meta's open-weight large language model family. Popular for research and fine-tuning.         | `open`, `research`, `local`, `LLM`         |
| **[GPT-Neo/GPT-J](https://huggingface.co/EleutherAI)**   | Open LLMs from EleutherAI. Can be run locally or hosted via HuggingFace.                      | `LLM`, `open`, `education`, `poetry`       |
| **[StableLM](https://github.com/Stability-AI/StableLM)** | Stability AI's open-source LLM series for local generation tasks.                             | `creative`, `open`, `local`, `LLM`         |

## 🛠️ Local Deployment Tools
| Tool/Platform                                       | Description                                                                | Tags                                    |
| --------------------------------------------------- | -------------------------------------------------------------------------- | --------------------------------------- |
| **[Ollama](https://ollama.com/)**                   | Simple command-line tool to run open LLMs locally with minimal setup.      | `local`, `LLM`, `easy`, `developer`     |
| **[LocalAI](https://github.com/go-skynet/LocalAI)** | Open-source alternative to OpenAI APIs, compatible with many local models. | `open`, `api-compatible`, `offline`     |
| **[LM Studio](https://lmstudio.ai/)**               | GUI for running and experimenting with local LLMs, great for non-coders.   | `LLM`, `GUI`, `offline`, `experimental` |

---

## 🌐 API-Only / Cloud-Based Models

Require API keys or subscriptions to use—less transparent, but powerful and production-ready.

| Tool/Platform                                                     | Description                                                                   | Tags                                              |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------------- | ------------------------------------------------- |
| **[OpenAI GPT-4 / ChatGPT](https://platform.openai.com/)**        | Industry-leading closed-source LLM with chat, code, and multimodal support.   | `closed`, `LLM`, `creative`, `education`          |
| **[Google Gemini](https://deepmind.google/technologies/gemini/)** | Multimodal model suite (text, image, audio) via Bard or Vertex AI API.        | `closed`, `multimodal`, `AI writing`, `education` |
| **[Cohere](https://cohere.com/)**                                 | API-first platform for LLMs, classification, semantic search, and embeddings. | `LLM`, `commercial`, `API`, `education`           |
| **[ElevenLabs](https://www.elevenlabs.io/)**                      | High-fidelity text-to-speech API with voice cloning and multilingual support. | `TTS/voice`, `closed`, `API`, `creative`          |


---

## 🎨 Local & Artist-Friendly Tools

These tools are especially useful for workshops, teaching, or creative coding environments, ideal for artists, educators, and beginners exploring machine learning interactively.

| Tool                                                              | Description                                                                                 | Tags                                               |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| **[ml5.js](https://ml5js.org/)**                                  | Beginner-friendly ML library for the web using JavaScript and p5.js. Great for artists.     | `creative`, `education`, `TTS`, `vision`, `open`   |
| **[Wekinator](http://www.wekinator.org/)**                        | Real-time interactive ML via GUI; legacy tool still referenced in creative coding contexts. | `creative`, `education`, `interaction`, `gesture`  |
| **[Teachable Machine](https://teachablemachine.withgoogle.com/)** | No-code tool to quickly train models using webcam, audio, or pose—runs directly in-browser. | `education`, `TTS`, `gesture`, `visual`, `browser` |
| **[transformers.js](https://xenova.github.io/transformers.js/)**  | In-browser transformer models (e.g., text, image) compatible with JavaScript and p5.js.     | `LLM`, `open`, `browser`, `education`, `advanced`  |


---

## 🧩 Utility Platforms and Repositories

| Tool/Platform                                       | Description                                                                               | Tags                                             |
| --------------------------------------------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------ |
| **[HuggingFace](https://huggingface.co/)**          | Repository of pretrained models for text, vision, speech. Free APIs and local options.    | `open`, `API`, `hosted`, `LLM`, `education`      |
| **[Replicate](https://replicate.com/)**             | Deploy ML models via web-based UI and APIs. Hugely popular for stable diffusion and LLMs. | `creative`, `visual`, `closed`, `API`            |
| **[Papers with Code](https://paperswithcode.com/)** | Academic paper tracker with code and benchmarks.                                          | `research`, `open`, `comparison`, `experimental` |

---

## 🏷️ Tags Glossary

| Tag         | Meaning                                            |
| ----------- | -------------------------------------------------- |
| `LLM`       | Large Language Model                               |
| `TTS/voice` | Text-to-Speech / Voice generation or transcription |
| `open`      | Fully open weights or open source code             |
| `closed`    | Closed-source, API only                            |
| `local`     | Can be run offline / on personal machine           |
| `API`       | Hosted, requires a key                             |
| `creative`  | Optimized for artistic, generative, or poetic work |
| `education` | Beginner-friendly or designed for teaching         |
| `visual`    | Focused on computer vision, image/video            |
| `gesture`   | Motion, pose, or interaction input                 |
| `research`  | Used in scholarly or experimental work             |

---

## 📌 Suggested Use Cases

- **Education**: ml5.js, Teachable Machine, Wekinator
- **Creative writing / poetry**: GPT-Neo, GPT-4, LLaMA, RunwayML
- **Audio/voice projects**: Whisper, Gemini, RunwayML TTS
- **Bias/Audit tools**: HuggingFace zero-shot models, Cohere classify
- **Custom input devices**: Wekinator, Teachable Machine, ml5.js + p5

---

## 📚 Additional Resources

### Nicky Case
- [AI Safety Dance (interactive explainer)](https://aisafety.dance/)
- [“June 2025: AI Therapists & AI Clones! 🤖” – Patreon post](https://www.patreon.com/posts/june-2025-ai-ai-131748990)

### Empire of AI
- [**Empire of AI: Decolonizing Artificial Intelligence** by Kate Crawford](https://mitpress.mit.edu/9780262048379/empire-of-ai/)  
  A forthcoming book exploring how AI systems reproduce and extend colonial power structures. Published by MIT Press (2024).

### Retrieval-Augmented Generation (Context Engineering)
- [NotebookLM (Google)](https://notebooklm.google.com/)
- [notebookllama (GitHub)](https://github.com/run-llama/notebookllama)
- [open-notebook (GitHub)](https://github.com/lfnovo/open-notebook)

----

## ✒️ Attribution

This tool guide is a companion to the _Supplemental Resource Guide_ for _Computational Text from A to Z_ and part of the **Equitable Syllabus Project** at NYU ITP. Contributions welcome.
