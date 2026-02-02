# 🛠️ HireCraft: Automated Job Application Pipeline

**HireCraft** is a production-ready, AI-driven system designed to automate the tedious process of tailoring resumes and cover letters. It uses LLMs to bridge the gap between a candidate's experience and a job's specific requirements.

## 🚀 The Vision
To build a modular system where a user provides a "Source of Truth" (Master Resume) and a target (Job URL), and receives a high-quality, ATS-optimized LaTeX resume and PDF in seconds.

---

## 🏗️ System Architecture
The system consists of a **FastAPI** backend for orchestration, **Celery/Redis** for asynchronous processing, and a **React** frontend for the dashboard.



---

## 🗺️ Project Roadmap (Phases)

### Phase 1: Foundation & Environment 🏗️
- [ ] Setup Dockerized environment (Python, Node, Postgres, Redis).
- [ ] Configure LaTeX (XeLaTeX/Tectonic) environment for PDF generation.
- [ ] Define the **Master Resume JSON** schema.

### Phase 2: Core Engine (The "Craft") ⚙️
- [ ] Build the **Job Scraper** (URL to Clean Text).
- [ ] Implement **LaTeX Injection** logic using Jinja2 templates.
- [ ] Create the **PDF Compiler** service.

### Phase 3: AI Intelligence 🧠
- [ ] Integrate LLM APIs (Gemini/OpenAI) via LiteLLM.
- [ ] Prompt Engineering: **Requirement Extractor**.
- [ ] Prompt Engineering: **Experience Optimizer** (ATS Keyword Injection).
- [ ] Hallucination Guardrails (ensuring dates/titles stay truthful).

### Phase 4: Frontend Dashboard 🖥️
- [ ] Resume/Template upload management.
- [ ] Job Application Tracker (Board view).
- [ ] Live "Diff" view (Original vs. AI-Optimized).
- [ ] Token usage & Cost tracking visualization.

### Phase 5: Deployment & Scale 🌐
- [ ] CI/CD Pipeline.
- [ ] Secure File Storage (S3 Integration).
- [ ] Rate limiting and user authentication.

---

## 🛠️ Tech Stack
* **Backend:** FastAPI (Python)
* **Worker:** Celery + Redis
* **LLM:** Gemini 1.5 Flash / GPT-4o
* **Typesetting:** XeLaTeX
* **Database:** PostgreSQL
* **Frontend:** React + Tailwind CSS
