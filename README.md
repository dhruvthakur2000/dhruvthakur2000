<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=00FFCC&center=true&vCenter=true&width=435&lines=Hi+%F0%9F%91%8B%2C+I%27m+Dhruv+aka+PsyRar.;AI+%7C+ML+%7C+Voice+Systems+Engineer;Building+real+systems%2C+not+demos.)](https://git.io/typing-svg)

</div>

---

### 🌌 About Me

***I publicly engineer real-world AI systems from scratch — documenting decisions, failures, tradeoffs, and mental models along the way.***

---

### 🚀 Flagship Project — SaleTech

> **Real-time AI voice sales agent. 40+ concurrent calls. Sub-600ms end-to-end latency. Zero vendor lock-in.**

| Component | Technology | Latency |
|---|---|---|
| Voice Activity Detection | Silero VAD v5 + WebRTC (dual-fusion) | 6ms |
| Speech Recognition | Faster-Whisper Large-v3 (streaming) | 150ms |
| Language Model | Qwen-2.5-7B-Instruct + KV-cache reuse | 320ms |
| Text-to-Speech | Piper TTS (streaming, sentence-by-sentence) | 100ms |
| **End-to-End P95** | | **~580ms** |

**What makes it different:**
- 🔁 **KV-cache reuse across turns** — 40% LLM latency reduction by serializing attention tensors to Redis
- 🎤 **Adaptive end-of-turn detection** — learns speaking pace per session; 420ms–720ms dynamic silence threshold
- ⚡ **Barge-in handling** — multi-signal fusion detects interruptions in <200ms, stops TTS mid-sentence
- 🧱 **Redis-backed session persistence** — full state, KV-cache, metrics per session; horizontal scaling ready
- ☸️ **Kubernetes-ready** — StatefulSet, HPA auto-scaling, PSTN via Asterisk/FreeSWITCH

**Stack:** `Python` `FastAPI` `AsyncIO` `WebSockets` `Silero` `Faster-Whisper` `PyTorch` `Redis` `Docker` `Kubernetes`

→ [`github.com/dhruvthakur2000/SaleTech`](https://github.com/dhruvthakur2000/SaleTech)

---

### 🔭 Projects

| Project | What it does | Stack |
|---|---|---|
| [**SaleTech**](https://github.com/dhruvthakur2000/SaleTech) | Production real-time AI voice sales agent — 40+ concurrent calls, <600ms latency, full open-source pipeline | Python · FastAPI · Silero · Faster-Whisper · Qwen · Piper · Redis · K8s |
| [**linux_driver_eval**](https://github.com/dhruvthakur2000/linux_driver_eval) | CLI framework to benchmark how well LLMs write Linux kernel device driver code. Two pipelines: generation + evaluation. Weighted scoring across correctness, security, quality, performance | Python · GCC · Together API · Static Analysis |
| [**virtual-voicebot**](https://github.com/dhruvthakur2000/virtual-voicebot) | Streamlit voice assistant with persona-aware responses — the project that started my obsession with real-time audio pipelines | Python · Streamlit · Groq · Whisper · LLaMA · TTS |
| 🔜 **HomeAssist** *(planned)* | Smarter Alexa — always-on edge voice assistant using SaleTech's VAD + ASR + buffer layers. Wake-word detection, local LLM, zero cloud dependency | SaleTech core · Edge inference |
| 🔜 **SaleTech Analytics** *(planned)* | Call intelligence layer — real-time sentiment, objection detection, sales stage classification per turn | SaleTech core · NLP · Classification |

---

### 🧠 Skills & Tech Stack

#### ⚙️ Languages & Tools
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/linux-%23000000.svg?style=for-the-badge&logo=linux&logoColor=white)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

#### 📊 ML & Data Science
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0C1A30?style=for-the-badge&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-008080?style=for-the-badge&logo=matplotlib&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

#### 🤖 GenAI & LLM Stack
![LangChain](https://img.shields.io/badge/LangChain-000000?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=for-the-badge&logo=langchain&logoColor=00FFCC)
![Hugging Face](https://img.shields.io/badge/Huggingface-%23FFD21F.svg?style=for-the-badge&logo=huggingface&logoColor=black)
![ChromaDB](https://img.shields.io/badge/ChromaDB-101010?style=for-the-badge&logo=vector&logoColor=white)
![QLoRA](https://img.shields.io/badge/QLoRA-262626?style=for-the-badge&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-Retrieval_Augmented_Gen-6DB33F?style=for-the-badge&logoColor=white)
![AI Agents](https://img.shields.io/badge/AI_Agents-Agentic_Systems-00FFCC?style=for-the-badge&logoColor=black)
![Multi-Agent](https://img.shields.io/badge/Multi--Agent_Systems-FF6B6B?style=for-the-badge&logoColor=white)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-Advanced-blueviolet?style=for-the-badge&logoColor=white)
![Function Calling](https://img.shields.io/badge/Function_Calling-Tool_Use-orange?style=for-the-badge&logoColor=white)
![Fine-tuning](https://img.shields.io/badge/Fine--Tuning-LLMs-red?style=for-the-badge&logoColor=white)

#### 🎙️ Voice AI (Specialist Stack)
![Silero VAD](https://img.shields.io/badge/Silero_VAD-v5-00FFCC?style=for-the-badge)
![Faster Whisper](https://img.shields.io/badge/Faster--Whisper-Large--v3-00FFCC?style=for-the-badge)
![Piper TTS](https://img.shields.io/badge/Piper_TTS-Neural-00FFCC?style=for-the-badge)
![WebRTC VAD](https://img.shields.io/badge/WebRTC_VAD-Dual_Fusion-00FFCC?style=for-the-badge)
![Streaming ASR](https://img.shields.io/badge/Streaming_ASR-Real--Time-00FFCC?style=for-the-badge)

#### 🌐 Backend & APIs
![FastAPI](https://img.shields.io/badge/fastapi-005571?style=for-the-badge&logo=fastapi)
![REST API](https://img.shields.io/badge/REST%20API-6DB33F?style=for-the-badge&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-Async-informational?style=for-the-badge)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![AsyncIO](https://img.shields.io/badge/AsyncIO-Concurrent-3776AB?style=for-the-badge&logo=python&logoColor=white)

#### ☁️ Infrastructure & DevOps
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![MLOps](https://img.shields.io/badge/MLOps-Learning_Next-FFD700?style=for-the-badge&logoColor=black)

---

### 📍 Pins & Badges

[![An image of @dhruvthakur2000's Holopin badges, which is a link to view their full Holopin profile](https://holopin.me/dhruvthakur2000)](https://holopin.io/@dhruvthakur2000)

---

### ✍️ Writing

I write about real engineering decisions — not tutorials copied from docs.

| | Post | Platform |
|---|---|---|
| 📡 | [VAD: Voice Activity Detection — how it actually works](https://vad-voice-activity-detection.hashnode.dev/vad-voice-activity-detection) | Hashnode |
| 🔁 | [Understanding the Attention Mechanism: The Heart of the Transformer Revolution](https://medium.com/@dhruvshirar/understanding-the-attention-mechanism-the-heart-of-the-transformer-revolution-51c6acb69edd) | Medium |
| 🪵 | [Structured Logging in Python: A Practical Guide for Production Systems](https://medium.com/@dhruvshirar/structured-logging-in-python-a-practical-guide-for-production-systems-9659f461fa93) | Medium |

---

### 📊 GitHub Stats

<div align="center">

![Dhruv's GitHub Stats](https://github-readme-stats.vercel.app/api?username=dhruvthakur2000&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=00FFCC&icon_color=00FFCC)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=dhruvthakur2000&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=00FFCC)

![GitHub Streak](https://streak-stats.demolab.com?user=dhruvthakur2000&theme=radical&hide_border=true&background=0D1117&ring=00FFCC&fire=00FFCC&currStreakLabel=00FFCC)

</div>

---

### 🤝 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/dhruv-thakur-2000)
[![X / Twitter](https://img.shields.io/badge/X_%40psyrar__-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/Dhruv_Thakur__)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@dhruvshirar)
[![Hashnode](https://img.shields.io/badge/Hashnode-2962FF?style=for-the-badge&logo=hashnode&logoColor=white)](https://hashnode.com/@dhruvthakur2000)
[![Email](https://img.shields.io/badge/dhruvshirar%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhruvshirar@gmail.com)

</div>

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=dhruvthakur2000&color=00FFCC&style=flat-square&label=profile+views" />
  <br><br>
  <i>Open to ML Engineer / AI Engineer / Backend Python roles — remote or on-site.</i>
  <br><br>
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
</div>
