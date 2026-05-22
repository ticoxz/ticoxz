# Hi there, I'm Marcelo (Tico) Miranda 👋

### Frontend Engineer | React & Next.js Specialist

I am a software engineer based in **Santiago, Chile**, with **4+ years of experience** building scalable, high-performance web applications. My focus is on creating exceptional user experiences using modern architectures and integrating cutting-edge AI solutions into products.

Currently, I specialize in the **React ecosystem**, leveraging **Next.js (App Router)**, **TypeScript**, and **Chrome Extensions** to build robust, innovative SaaS products. I also have strong experience setting up **CI/CD pipelines**, state management architectures, and integrating complex APIs.

---

## 🛠️ Tech Stack & Tools

**Frontend Core**
![React](https://img.shields.io/badge/-React-61DAFB?style=flat&logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat&logo=next.js&logoColor=white) ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat&logo=vite&logoColor=white)

**Backend & AI**
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat&logo=node.js&logoColor=white) ![Groq](https://img.shields.io/badge/-Groq_SDK-f97316?style=flat) ![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat&logo=prisma&logoColor=white) ![Supabase](https://img.shields.io/badge/-Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white) ![CLI](https://img.shields.io/badge/-CLI_Tooling-000000?style=flat)

**State & UI Design**
![Zustand](https://img.shields.io/badge/-Zustand-orange?style=flat) ![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white) ![Framer Motion](https://img.shields.io/badge/-Framer_Motion-0055FF?style=flat&logo=framer&logoColor=white) ![Figma](https://img.shields.io/badge/-Figma-F24E1E?style=flat&logo=figma&logoColor=white)

**Infrastructure & Services**
![Google Cloud](https://img.shields.io/badge/-Google_Cloud-4285F4?style=flat&logo=google-cloud&logoColor=white) ![Clerk](https://img.shields.io/badge/-Clerk_Auth-6C47FF?style=flat&logo=clerk&logoColor=white) ![Stripe](https://img.shields.io/badge/-Stripe-008CDD?style=flat&logo=stripe&logoColor=white)

---

## 🚀 Featured Projects

### 🍌 [BananaBridge - AI Meeting Copilot](https://b-bridge.app/)
*An advanced AI-powered "Copilot" for Google Meet that completely eliminates language barriers, boosts interview confidence, and automates meeting workflows.*

* **The Problem:** Latency in real-time translation, generic AI responses, and lack of contextual intelligence during high-stakes remote meetings.
* **The Solution:** A sophisticated **React+Vite Chrome Extension** paired with a **Next.js Fullstack Dashboard**. It reads the DOM (MutationObserver), proxies requests securely, and uses ultra-low latency LLMs for instant conversational support.
* **The Stack:** Next.js 14, React, TypeScript, Tailwind CSS, Framer Motion, Zustand, Groq Cloud (LLaMA v3.3), Deepgram Nova 3, Clerk Auth, Stripe.

**🔥 Key Features:**
* 🎭 **Dynamic AI Personas:** Choose roles like "Senior Engineer", "Product Manager", or "Account Executive" to get tailored, jargon-accurate smart replies.
* 🧠 **Personal Context Injection:** Upload your CV/PDF directly to the extension. The AI digests your exact profile to answer interview questions using your actual background.
* 💼 **Interview & Technical Modes:** Adapts the response format automatically—from short tactical answers to full STAR-method (Situation, Task, Action, Result) interview scripts.
* 🎬 **Director Mode (Memory):** Automatically persists conversation history. You can asynchronously ask the Director to "write Jira tickets based on what we just discussed".
* 🎧 **Speaker Diarization:** Uses Deepgram API for 54% higher accuracy and real-time multilingual speaker recognition instead of relying solely on Google Meet captions.
* 💳 **Full Monetization Cycle:** Complete integration with Clerk authentication, Pro user entitlements, usage limits, and Stripe subscriptions.

### 🔁 [Relay — Git for AI sessions](https://github.com/ticoxz/Relay)
*Open-source CLI to checkpoint, encrypt, and share AI coding context across editors and teammates — like Git, but for the reasoning behind your code.*

* **The Problem:** Cursor, VS Code Copilot, OpenCode, and Antigravity keep hours of decisions, trade-offs, and file context in proprietary local storage. When you switch machines, editors, or start a fresh chat, that thread is gone — even though your repo has the diff.
* **The Solution:** A **TypeScript CLI** that reads sessions from supported editors, normalizes them to a standard JSON format, encrypts with **[age](https://github.com/FiloSottile/age)** + team SSH keys, writes to `.ai-memory/` in your project, and generates **`.ai-memory/HANDOFF.md`** for the next human or agent.
* **The Stack:** Node.js, TypeScript, age encryption, Git hooks, modular readers/injectors (Cursor, VS Code, OpenCode, Antigravity).

**🔥 Key Features:**
* 👥 **Team relay:** `relay sync --handoff` → commit `HANDOFF.md` → teammate runs `git pull` and continues where you left off.
* 🔀 **Editor bridge:** `relay inject cursor antigravity` (or VS Code ↔ Cursor) when native import APIs don't exist — `@path` handoff instead of starting from zero.
* 🔄 **Context window reset:** Save game with `relay sync --handoff`, open a new chat, attach `@.ai-memory/HANDOFF.md` — no re-explaining the whole architecture.
* 🔐 **Local-first security:** Sessions encrypted per team SSH keys; raw chats stay gitignored, handoff + config travel with the repo.
* 📦 **Install:** `npm install -g @ticoxz/relay` · [docs & quickstart](https://github.com/ticoxz/Relay#quickstart)

### 🧠 [Animus — Cognitive companion on Telegram](https://github.com/ticoxz/Animus)
*Personal AI second brain in Telegram: persistent memory, agent tools, custom skills, and an interactive knowledge graph — built for real life, not work dashboards.*

* **The Problem:** Chatbots forget context, mix languages, can't tie conversations to calendar or long-term goals, and don't give users a visual map of what they "know" about you.
* **The Solution:** A **Next.js 15** app with **Telegram webhook**, **Supabase** memory bank (facts, entities, relations), **MiniMax/OpenAI** agent loop with tools, **runtime skills** users create in natural language, and a **`/mind` web graph** (JWT from Telegram).
* **The Stack:** Next.js 15, TypeScript, Supabase, MiniMax API, Telegram Bot API, Google Calendar OAuth, react-force-graph-2d, Docker/VPS deploy.

**🔥 Key Features:**
* 🧠 **Agent mode:** `search_memory_facts`, past chats, weather, web search, Google Calendar read/create, custom skills.
* 📅 **Calendar:** OAuth + `/agenda` + natural language scheduling (`Drimo 25/5 at 11`).
* 🕸️ **Mind graph:** Interactive entity map with search, zoom, per-user voice style (e.g. Paraguayan Spanish).
* 🧩 **Runtime skills:** "I want a skill that…", migrate chat to skill, curator archives unused skills, SKILL.md export.
* 💾 **Memory:** Auto fact extraction, `/memory`, selective forget, identity answers as short summaries (not raw profile dumps).
* 🚀 **Deploy:** Local ngrok dev, Vultr/Hetzner VPS 24/7 — [full README](https://github.com/ticoxz/Animus).

---

## 💼 Professional Highlights

**Frontend Engineer @ Tucar (4 years)**
* 🔐 **Authentication System:** Developed the frontend for the new Auth System from scratch, refactoring it to TypeScript and integrating it seamlessly into the corporate Monorepo.
* 🏢 **Corporate Web Development:** Led the development of the main corporate website, translating complex Figma designs into pixel-perfect, responsive code using Next.js.
* 🧩 **Architecture:** Developed the internal component library using **Storybook** to ensure design consistency across all applications.
* ☁️ **DevOps:** Designed and implemented automated CI/CD pipelines on Google Cloud Platform, significantly reducing deployment times and improving stability.

---

## ⚡ Fun Fact

🎧 When I'm not coding, I'm a **DJ and Music Producer**. I love finding the intersection between the logic of programming and the creativity of music production.

Check out my DJ sets here: [▶️ @ticobeatz](https://www.youtube.com/@ticobeatz)

---

<div align="center">
  
  📫 **Let's connect:** [ticomiranda4@gmail.com](mailto:ticomiranda4@gmail.com) | [BananaBridge](https://b-bridge.app/) | [Relay](https://github.com/ticoxz/Relay) | [Animus](https://github.com/ticoxz/Animus)

</div>
