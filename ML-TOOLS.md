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

---

## 🌐 API-Only / Cloud-Based Models

Require API keys or subscriptions to use—less transparent, but powerful and production-ready.

| Tool/Platform                                                     | Description                                                              | Tags                                             |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------ |
| **[OpenAI GPT-4 / ChatGPT](https://platform.openai.com/)**        | Leading closed-source LLM with natural dialogue and multi-modal support. | `closed`, `LLM`, `creative`, `education`         |
| **[Google Gemini](https://deepmind.google/technologies/gemini/)** | Multimodal models for voice, vision, and language (via Bard or API).     | `closed`, `TTS/voice`, `AI writing`, `education` |
| **[RunwayML](https://runwayml.com/)**                             | GUI-based creative ML platform—GPT, TTS, image gen, video tools.         | `closed`, `GUI`, `TTS`, `visual`, `creative`     |
| **[Cohere](https://cohere.com/)**                                 | API-based NLP tools for classification, generation, and embeddings.      | `LLM`, `commercial`, `API`, `education`          |

---

## 🎨 Local & Artist-Friendly Tools

These are especially useful for workshops, teaching, or creative coding environments.

| Tool                                                              | Description                                                                     | Tags                                               |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------- | -------------------------------------------------- |
| **[ml5.js](https://ml5js.org/)**                                  | Beginner-friendly ML for the web using JavaScript and p5.js. Great for artists. | `creative`, `education`, `TTS`, `vision`, `open`   |
| **[Wekinator](http://www.wekinator.org/)**                        | GUI for training ML models with real-time input/output (e.g., sensors).         | `creative`, `education`, `interaction`, `gesture`  |
| **[Teachable Machine](https://teachablemachine.withgoogle.com/)** | No-code tool to train simple models using webcam, audio, or pose data.          | `education`, `TTS`, `gesture`, `visual`, `browser` |

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

## ✒️ Attribution

This tool guide is a companion to the _Supplemental Resource Guide_ for _Computational Text from A to Z_ and part of the **Equitable Syllabus Project** at NYU ITP. Contributions welcome.
