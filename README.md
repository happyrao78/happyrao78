<div align="center">

# Happy Yadav

### AApplied AI Engineer · Voice AI Systems · Full-Stack Developer

Building production-grade real-time Voice AI pipelines, multi-agent LLM systems, and scalable backend platforms.

[![Portfolio](https://img.shields.io/badge/Portfolio-yadavhappy.in-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white)](https://www.yadavhappy.in)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/happy-yadav-16b2a4287)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:happy.yadav.ai@gmail.com)

</div>

---

## About Me

I'm a Applied AI Engineer and full-stack developer with hands-on **production experience** building real-time Voice AI systems, multi-channel conversational agents, and LLM-powered backend pipelines.

My core strength is architecting **end-to-end AI systems** — from low-latency voice-to-voice (V2V) streaming pipelines using LiveKit and WebRTC, to LangChain-orchestrated chatbot services with MCP-based enterprise tool integrations. On the full-stack side, I build scalable backend services with **Python/FastAPI** and frontend interfaces with **React**.

I specialize in agentic AI systems, RAG pipelines, multi-provider LLM routing, and real-time communication stacks — and I've shipped these in production across **web, WhatsApp, and telephony** channels.

- 🎙️ Currently building real-time **Voice AI** and **MCP-based AI assistant integrations** at **EaseMyTrip**
- 🧠 Deep focus on **STT → LLM → TTS** pipelines, multi-agent orchestration, and low-latency systems
- 🛠️ Working daily with **LangChain, LangGraph, LiveKit, FastAPI, and multi-provider LLM routing**
- ✍️ I write about real-time audio AI, LLM orchestration, and system-level optimization on X
- 🌱 Currently exploring **MCP / UCP protocol design** and cross-platform AI assistant widget delivery

---

## Current Focus Areas

```text
🎧  Real-time Voice AI            STT → LLM → TTS pipelines, V2V systems
📞  Telephony & WebRTC            LiveKit, Twilio, Exotel, VoIP protocol engineering
🤖  Multi-Agent Orchestration     LangChain, LangGraph, agent handoff architectures
⚡  Low-Latency Inference          Token-aware model routing, cost-optimized LLM switching
🏗️  Scalable Backend Systems      Async-first architecture, FastAPI, Docker, PostgreSQL
🔍  Applied RAG Systems           Vector search, Pinecone, FAISS, grounded Q&A
🔌  MCP / Agentic Tooling         Model Context Protocol integrations for ChatGPT & Claude
```

---

## Professional Experience

### Applied AI Engineer — EaseMyTrip.com
**Aug 2025 – Present · Gurugram, Haryana, India**

Architecting and delivering production-grade Conversational AI and Voice AI systems serving customers across **Web, WhatsApp, and Telephony** channels.

- Engineered and launched EaseMyTrip's **MCP integration for ChatGPT and Claude**, transforming internal travel APIs into production-grade MCP tools with conversational tool-calling support for bookings, itinerary management, and customer assistance directly inside ChatGPT and Claude.
- Designed and implemented a real-time voice streaming pipeline using **LiveKit (WebRTC)**, **Silero VAD**, **Groq Whisper STT**, and multi-provider TTS (ElevenLabs, Azure, Google Wavenet, Sarvam) — achieving **sub-900ms round-trip latency** through chunked audio streaming, adaptive buffering, and preemptive interruption handling.
- Engineered the **WhatsApp Travel Bot**, integrating Meta Webhook APIs, Redis-backed session management, and the core chatbot service for seamless multi-channel AI-driven travel assistance.
- Developed the **EMT Chatbot core service** with a dual-chain LangChain architecture: a tool-calling chain for intent classification and dynamic tool invocation, paired with a dedicated LLM summarization chain for structured, channel-aware responses.
- Contributed to the **EMT Tools Ecosystem** — an MCP-based tool-calling framework powering flight search, hotel lookup, train/bus booking, pre/post-booking flows, and OTP-based authentication.
- Applied **DeepFilterNet** for real-time noise suppression and conducted R&D across OpenAI, Gemini, Anthropic, Deepgram, Google, Sarvam, and Groq voice models — cutting per-call operational cost and improving inference throughput via token-aware routing.
- Practiced async-first development, containerized all services with **Docker**, and collaborated with DevOps on production deployment and scalability.

### Backend Developer Intern — Hunar.ai
**Gurugram, India**

- Designed and optimized **PostgreSQL query pipelines** for data extraction workflows serving 20+ enterprise clients with 100,000+ records, improving reporting efficiency by **30%**.
- Built RESTful APIs and contributed to schema optimization, reducing query execution time across core reporting modules.
- Explored LLM integration patterns and contributed to backend modules supporting AI-assisted features within the platform.

### Technical Lead — Coding Ninjas Club, Chitkara University
**2024 – 2025 · Punjab, India**

- Led technical workshops and mentored **100+ club members** on AI/ML, full-stack development, and competitive programming.
- Organized hackathons, coding sprints, and project showcases, fostering a culture of applied engineering and product thinking.
- Guided juniors in building production-ready AI and web projects, strengthening the club's presence at university and national levels.

---

## Featured Work & Projects

### 🎧 ComplaintHub — V2V Voice Pipeline for Citizen Grievance Automation
A fully automated voice-to-voice citizen complaint registration system — users interact entirely through natural speech over a live call, with **no human agent involved**. The pipeline ingests live audio, transcribes via ASR, reasons over an LLM, and delivers a synthesized spoken response end-to-end.

- Real-time audio stack using **GPT-4o-mini-realtime-preview** streaming for telephony (Twilio/Exotel), with custom G.711 µ-law converters, jitter buffer tuning, RTP optimization, and FFmpeg preprocessing.
- POC across **three voice pipeline architectures**: OpenAI GPT-4o Realtime (PCM16 WebSocket), Gemini Native Audio Thinking Model, and a custom STT–LLM–TTS micro-pipeline (Whisper → Groq GPT-OSS → Google Wavenet) — with token-aware routing and latency-based model swapping.
- **Silero VAD** with server-side threshold tuning + **DeepFilterNet** noise suppression, eliminating false-trigger interruptions in noisy call environments.
- Multi-stage NLP extraction for citizen intent, complaint category, and brand details — persisted to Redis with async PostgreSQL for durable storage.

### 📊 Syntropy Labs — LLM Evaluation & Benchmarking Platform
A four-microservice LLM evaluation platform: an **Orchestrator** (API gateway, JWT auth, org/project management, job orchestration), a **Model Runner** (FastAPI + LiteLLM multi-provider proxy), an **Eval Engine** (automated metric scoring), and MongoDB for metadata persistence.

- Provider-agnostic inference proxy via **LiteLLM**, normalizing OpenAI, Anthropic, Gemini, Mistral, and Azure into a single OpenAI-compatible interface with per-provider token and latency tracking.
- WebSocket-based **Realtime Service** for live voice evaluation, integrating OpenAI Realtime API and Gemini BidiGenerateContent for audio-in/audio-out benchmarking.
- **Eval Engine** supporting statistical metrics, predefined LLM-as-judge metrics (relevance, groundedness, coherence, fluency), and fully custom criteria with configurable judge model, threshold, and per-metric weighting.
- Multimodal evaluation pipelines for AI-generated image/video — scoring physics plausibility, anatomical correctness, semantic adherence, temporal consistency, and aesthetic quality via vision-capable LLM evaluators.
- Progressive batch evaluation system with per-row score persistence to GCS-hosted CSV datasets, enabling real-time progress polling and partial recovery on mid-job failures.

### 🌐 EaseMyTrip ChatGPT App & Claude Connector
Led the integration of EaseMyTrip's travel services into **ChatGPT and Claude via the Model Context Protocol (MCP)**.

- Exposed enterprise travel APIs as production-ready MCP tools for flight search, hotel discovery, itinerary planning, booking assistance, and post-booking operations through natural conversation.
- Architected a **cross-platform widget delivery framework** dynamically serving Claude-optimized experiences from a unified backend, API layer, and business logic.
- Designed secure MCP tool integration, parameter extraction pipelines, and channel-aware conversational workflows for enterprise-grade reliability.

### 🎬 Aura.ai — Text-to-Video AI SaaS Platform
An AI SaaS platform automating end-to-end video creation from text/document inputs — covering LLM-powered summarization, multilingual voiceover synthesis, sign-language video generation, and AR/VR scene integration for accessibility in education and corporate training.

- **AuraBot** — a knowledge-base-grounded RAG assistant for contextual Q&A over uploaded course/training material.
- Analytics dashboard tracking viewer engagement, quiz completion, comprehension scores, and retention — personalizing content delivery per learning profile.

### ✈️ Ninja Navigator AI — Multi-Agent Travel Planning System
A production-grade multi-agent system orchestrating **five specialized agents** with asynchronous coordination and persistent state management.

- Built with LangChain, LangGraph, and FastAPI; enterprise-grade practices including structured logging, exception handling, CI/CD, UV package management, and Husky git hooks.
- Multi-provider LLM integration (OpenAI, Groq) with concurrent asyncio workflows — **~95% uptime**.

### 🏢 Sankalpiq — Multi-Agent AI Automation Suite
An enterprise-grade AI automation platform with autonomous micro-agents for email automation, voice-based FAQ/data collection, WhatsApp outreach, and analytics dashboards.

- Built on LLMs, FastAPI, Docker, Pinecone, and LangChain orchestration with semantic search and real-time telephonic interactions.
- Delivered **~50% operational efficiency gains** and **40% higher stakeholder engagement**.

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**AI / ML & Agentic Systems**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LangSmith](https://img.shields.io/badge/LangSmith-1C3C3C?style=flat-square)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square)
![MCP](https://img.shields.io/badge/Model%20Context%20Protocol-MCP-6E56CF?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-Retrieval%20Augmented%20Generation-FF6F00?style=flat-square)

**Voice & Real-Time Systems**

![LiveKit](https://img.shields.io/badge/LiveKit-WebRTC-FF3D00?style=flat-square)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-Audio%20Streaming-010101?style=flat-square&logo=socketdotio&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)

**Backend & Infrastructure**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Tooling & Platforms**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![GCP](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)

---

## Skillset Breakdown

| Category | Skills |
|---|---|
| **Languages** | Python, JavaScript, TypeScript, C++, SQL |
| **Frameworks & Libraries** | FastAPI, React, Node.js, Express.js, Redux, Streamlit, Selenium, BeautifulSoup |
| **AI & ML** | LangChain, LangGraph, LangSmith, RAG, LLM Embeddings, Prompt Engineering, MCP, UCP, Pinecone, FAISS, OFGA |
| **Voice & Real-Time** | LiveKit (WebRTC), ASR, WebSocket Audio Streaming, VAD, Speaker Diarization, STT/TTS pipelines, DeepFilterNet, Twilio, Exotel, µ-law, FFmpeg, Opus |
| **Databases** | PostgreSQL, MongoDB, Redis, SQLite, Firestore |
| **Tools & Platforms** | Git, Docker, Google Cloud, Firebase, LiteLLM, UV, Husky, Ngrok, Cloudflare |
| **Architecture** | REST APIs, Microservices & Monolithic Architecture, Async Pipelines, CI/CD |

---

## Achievements

🏆 **Top 22 National Finalist & Social Buzz Winner** — Bajaj Finserv HackRx 5.0
🏆 **Top 50 Finalist** — Cars24 Token'26 (hosted by OpenAI, AWS & ElevenLabs)
🏆 **Winner** — Aditya Birla Group's Synaptix Hackathon '25 (Delhi Technological University)
🏆 **Selected** — GitHub Field Day '24 at Microsoft, Gurgaon
🏆 **First Runner-Up** — FusionFest Hackathon, Chitkara University
🏆 **Finalist & Social Buzz Winner** — Vihaan 7.0, Delhi Technological University

---

## Education

**Bachelor of Computer Applications — Information Technology**
Chitkara University, Punjab, India · CGPA: 9.12

---

## Let's Connect

I'm interested in roles and collaborations involving **Applied AI**, **Voice AI**, **LLM Systems**, and **scalable backend engineering** — and I'm open to research-driven engineering problems and early-stage product work.

[![Portfolio](https://img.shields.io/badge/Portfolio-yadavhappy.in-2563EB?style=for-the-badge)](https://www.yadavhappy.in)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/happy-yadav-16b2a4287)
[![Gmail](https://img.shields.io/badge/Email-happy.yadav.ai%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:happy.yadav.ai@gmail.com)

---

<div align="center">
<sub>⭐ If you found my work interesting, consider checking out my pinned repositories below.</sub>
</div>
