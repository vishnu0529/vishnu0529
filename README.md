<div align="center">

# Hi, I'm Vishnu 👋

### Taking AI agents from pilot to production: evals, cost control, data boundaries

[![Portfolio](https://img.shields.io/badge/Portfolio-vishnu0529.github.io-0ea5e9?style=for-the-badge&logo=google-chrome&logoColor=white)](https://vishnu0529.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vishnu-kanth-suryanarayan-a68851167)
[![Email](https://img.shields.io/badge/Email-vishnuks0529@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vishnuks0529@gmail.com)
[![Resume](https://img.shields.io/badge/📄_Paper_Trail-EA4335?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](https://github.com/vishnu0529/vishnu0529/raw/main/Vishnu_AI_Engineer_CV_1.pdf)

</div>

---

I work on the part of AI agents that decides whether they survive contact with a real business: evaluation, cost per task, data boundaries, escalation paths, and who owns the thing once it ships. Most agent pilots don't fail on model quality. They fail because nobody set an acceptance threshold, nobody measured cost per task, nobody defined what happens when the agent is wrong.

**What I'm working on**
- Agent orchestration on LangGraph: typed state, a critique/re-plan cycle, durable Postgres checkpointing that survives a killed process, and a genuine `interrupt()` human-in-the-loop gate on commercially sensitive actions
- Evaluation as a CI merge gate, not a notebook: golden sets with adversarial traps, acceptance thresholds, CI that fails the PR on regression
- Tracing, cost-per-task, and config/prompt versioning, so every answer is traceable to the exact commit that produced it

**What I don't claim**
- AutoGen and CrewAI: read, not shipped
- Anything below is built, hardened and tested. Where something is on staging rather than in production, the repo's own README says so

MSc AI & Robotics, University of Hertfordshire · ex-Deloitte Digital Senior Consultant · London

Open to AI engineering roles in London, and to short production-readiness reviews for firms with an agent pilot that hasn't shipped.

---

## 🚀 Featured Projects

| Project | What it does | Stack | Status |
|---|---|---|---|
| 🧠 **[Proposal Response Assistant](https://github.com/vishnu0529/enterprise-rag-assistant)** | Multi-agent LangGraph system for professional-services bid teams: a Retrieval Strategist and Drafting Agent share graph state; citation enforcement and escalation on ungrounded answers; a real `interrupt()` pause on commercially-sensitive answers; durable Postgres checkpointing verified with a live two-process, real-`SIGKILL` demo; OpenTelemetry tracing per node; a 50-item golden set with 12 adversarial traps in a CI merge gate. Scored against a public [15-point production-readiness scorecard](https://claude.ai/code/artifact/5c6af602-27b4-4bc1-af7b-c2cb501da89c) (9 demonstrated, 5 partial, 1 open; self-assessed, not 15/15). | LangGraph · Postgres · Qdrant · OpenTelemetry · FastAPI | [![Live](https://img.shields.io/badge/-Live-34d399?style=flat-square)](https://enterprise-rag-assistant-iyq9apbv2jeyby3xxqx3ce.streamlit.app/) |
| 🟦 **[RFP Agent (TS)](https://github.com/vishnu0529/rfp-agent-ts)** | The TypeScript/Node counterpart to the Proposal Response Assistant, with the same durable Postgres checkpointing and genuine `interrupt()` human-in-the-loop gate, proven in LangGraph.js rather than LangGraph Python, with the same real kill-and-resume demo (SIGKILL a live process, resume from checkpoint in a second process). Proves the pattern isn't a Python-specific trick. | LangGraph.js · TypeScript · Node · Postgres | [![CI](https://img.shields.io/badge/-CI_passing-34d399?style=flat-square)](https://github.com/vishnu0529/rfp-agent-ts/actions) |
| 🔍 **[AI Job Finder Bot](https://github.com/vishnu0529/ai-job-finder-bot)** | Multi-board job search with a LangGraph agent: scores each result, drafts a cover letter, critiques its own draft and re-writes if it's not grounded, remembers past applications across sessions | LangGraph · Gemini · Streamlit · SQLite | [![Live](https://img.shields.io/badge/-Live-34d399?style=flat-square)](https://ai-job-finder-bot-bnqepy7obmunbihrkyxv4f.streamlit.app/) |
| 🤖 **[AI Resume Matcher](https://github.com/vishnu0529/ai-resume-matcher)** | 4-step agentic LLM pipeline that analyses a CV against any job description: skill extraction → gap analysis → tailored content generation → application strategy | Gemini 3.6 Flash + Claude · FastAPI · Render | [![Live Demo](https://img.shields.io/badge/-Live_Demo-34d399?style=flat-square)](https://ai-resume-matcher-afsgzlmmklspynzeebp9w4.streamlit.app) [![API](https://img.shields.io/badge/-API_Docs-0ea5e9?style=flat-square)](https://ai-resume-matcher-xw2i.onrender.com/docs) |

<details>
<summary><b>Other projects</b> (not in active development, kept for reference)</summary>
<br>

| Project | What it does | Stack |
|---|---|---|
| 🏆 [Sports AI Prediction API](https://github.com/vishnu0529/sports-ai-api) | Sports match prediction API using OpenAI, natural-language queries | FastAPI · OpenAI · Render |
| 📊 [Employee Sentiment Analysis](https://github.com/vishnu0529/Employee-Sentiment-Analysis) | NLP pipeline for sentiment classification + flight-risk detection on 2,200+ emails | BERT · VADER · scikit-learn |
| 🏥 [Federated Healthcare AI](https://github.com/vishnu0529/Federated_Project) | Privacy-preserving federated learning pipeline predicting hospital readmissions without centralising patient data | Flower (flwr) · scikit-learn |

*Note: the Sports AI API's C# rewrite ([sports-ai-api-csharp](https://github.com/vishnu0529/sports-ai-api-csharp)) was previously hosted on Railway; that deployment is currently down (Railway trial ended), repo/code is unaffected.*

</details>

---

## 📜 Certifications

- **Certificate of Attendance, From Zero to Hero: Federated AI in Healthcare Systems** · St John's College, Cambridge (24–25 Aug 2026) · hosted by Cambridge Image Analysis (DAMTP, University of Cambridge), PharosAI & Core AI · built on the Flower (flwr) framework used in [Federated Healthcare AI](https://github.com/vishnu0529/Federated_Project) above · [Verify credential](https://verified.sertifier.com/en/verify/99023372901934/)

---

## 🛠 Tech Stack

**LLM & Agentic AI**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white)
![Anthropic Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Multi-Agent Systems](https://img.shields.io/badge/Multi--Agent_Systems-8B5CF6?style=flat-square)
![Corrective RAG](https://img.shields.io/badge/Corrective_%2F_Self--RAG-8B5CF6?style=flat-square)
![Stateful Checkpointing](https://img.shields.io/badge/Durable_Checkpointing-8B5CF6?style=flat-square)
![Human in the Loop](https://img.shields.io/badge/Human--in--the--Loop-8B5CF6?style=flat-square)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-8B5CF6?style=flat-square&logo=opentelemetry&logoColor=white)

**Backend & APIs**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLModel](https://img.shields.io/badge/SQLModel-FF4B4B?style=flat-square)

**MLOps, Testing & DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

---

## 📈 GitHub Stats

<div align="center">

![Vishnu's GitHub Stats](https://github-readme-stats.vercel.app/api?username=vishnu0529&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1b2e&title_color=0ea5e9&icon_color=0ea5e9&text_color=94a3b8)
&nbsp;&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=vishnu0529&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1b2e&title_color=0ea5e9&text_color=94a3b8)

</div>

---

<div align="center">

**Open to AI engineering roles in London, and to short production-readiness reviews for firms with an agent pilot that hasn't shipped.**

⭐ Star a repo if you find it useful!

</div>
