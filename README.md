# Hi, I'm Ayush Vyas 👋

<p align="center">
  <em>CS student interested in AI engineering, backend development, and building useful AI applications.</em>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ayushvyas1">
    <img src="https://img.shields.io/badge/LinkedIn-ayushvyas1-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=AyushVyas8080&label=Profile+Views&color=0e75b6&style=flat" />
</p>

---

## 👨‍💻 About Me

- 🎓 BTech Computer Science student at **MAIT, Delhi**
- 🤖 Interested in **AI Engineering, LLMs, RAG, and AI agents**
- 🏗️ Building AI applications using **Python, FastAPI, LangGraph, PostgreSQL, and Next.js**
- 🧠 Enjoy working on backend systems, agent workflows, vector search, and LLM evaluation
- 🔍 Interested in making AI applications more reliable, secure, and cost-efficient
- ⚡ I learn best by building projects, testing them, and figuring out how things work.

---

## 🛠️ Tech Stack

- **Languages:** Python, SQL, TypeScript, JavaScript, C++
- **AI & LLMs:** RAG, LangChain, LangGraph, AI Agents, Embeddings, Vector Search, Prompt Engineering, LLM Guardrails
- **LLM APIs & Evaluation:** Groq, Google Gemini, Recall@k, MRR, LLM Evaluation
- **Backend:** FastAPI, Node.js, Express, REST APIs, Pydantic
- **Databases & Caching:** PostgreSQL, Supabase, Pinecone, pgvector, Redis, MongoDB
- **Tools:** Docker, Git, GitHub Actions, pytest, Linux, Prometheus, OpenTelemetry

---

## 🚀 Projects

### 🤖 AI Customer Support Agent

An AI-powered email support system that reads customer queries, searches company documents, and drafts replies based on relevant policies.

Some things I worked on:

- **Agent Workflow:** Used LangGraph to manage the agent's workflow, including document relevance checks, query rewriting, and retrying answers when the retrieved information isn't good enough.
- **Document Search:** Stored policy documents as 768-dimensional embeddings in Supabase PostgreSQL and used pgvector for semantic search.
- **AI Safety:** Added checks for prompt injection, sensitive information, and replies that make unauthorized promises about refunds, discounts, or callbacks.
- **Multiple LLMs:** Used Groq (`gpt-oss-120b`) for faster classification and Google Gemini (`gemini-2.5-flash`) for generating responses, with fallback support.
- **Email Integration:** Used Google Cloud Pub/Sub to receive Gmail updates through push webhooks. Added duplicate-message handling and automatic Gmail watch renewal.
- **Testing:** Added 42 unit tests, all passing, and tested the agent against 100 scenarios covering 11 different edge-case categories.

**Tech Stack:** Python · FastAPI · LangChain · LangGraph · Supabase pgvector · Groq · Google Gemini · GCP Pub/Sub · Next.js · Docker

**Links:**

[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://ai-customer-support-coral-eight.vercel.app/)
[![API Docs](https://img.shields.io/badge/API_Docs-009688?style=flat&logo=fastapi&logoColor=white)](https://ai-customer-support-jp8w.onrender.com/docs)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/ai-customer-support)

---

### 🛡️ LLM Guard — Secure LLM Gateway

A gateway for LLM applications that handles API requests, checks for security threats, and routes requests across different AI providers.

Some things I worked on:

- **Prompt Injection Detection:** Built multiple detection checks using Unicode normalization (NFKC), homoglyph detection, zero-width character removal, and pattern matching to catch attempts to bypass system instructions.
- **PII & Secret Detection:** Detects sensitive information such as AWS keys, GitHub tokens, JWTs, and payment card numbers. Uses Luhn checksum validation for credit card detection.
- **LLM Gateway:** Built an OpenAI-compatible `/v1/chat/completions` API that routes requests between Groq and Google Gemini, with circuit breakers and automatic fallbacks.
- **Rate Limiting & Caching:** Implemented Redis-based sliding-window rate limiting per API key and SHA-256 prompt hashing for exact-match cache lookups.
- **Request Tracing:** Tracks request latency, token usage, and estimated API costs, with asynchronous PostgreSQL trace storage.
- **Admin Dashboard:** Built a Next.js 16 dashboard with session management, API key management, and an interactive API playground.

**Tech Stack:** Python · FastAPI · Pydantic v2 · SQLAlchemy · PostgreSQL · Redis · Groq · Google Gemini · Structlog · Next.js · Docker

**Links:**

[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://guardllm.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/llmguard)

---

### 🔍 IncidentIQ — Incident Investigation Platform

A tool that helps investigate technical incidents by searching through runbooks, postmortems, and other engineering documents. It generates possible root causes and backs its findings with exact quotes from the source documents.

Some things I worked on:

- **Hybrid Search:** Combined PostgreSQL full-text search with Pinecone vector search using Reciprocal Rank Fusion (RRF).
- **Document Processing:** Built a background ingestion pipeline for runbooks, postmortems, architecture diagrams, and PDFs using ARQ and Redis.
- **Source Citations:** Generates root-cause hypotheses and read-only diagnostic steps, with quotes checked against the original documents.
- **LLM Fallbacks:** Uses Groq for responses and automatically switches to Gemini when needed, with retries and circuit breakers.
- **Search Evaluation:** Built an evaluation setup to measure Recall@k, Hit Rate, MRR, nDCG, citation accuracy, latency, and token costs.
- **Monitoring:** Added Prometheus metrics, structured logs, and OpenTelemetry tracing to monitor the application.

**Tech Stack:** Python · FastAPI · SQLAlchemy · Pinecone · NeonDB PostgreSQL · ARQ · Redis · OpenTelemetry · Prometheus · Next.js

**Links:**

[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://incidentiq-ai.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/incidentiq)

---

## 📚 Currently Learning

- Building more advanced AI agents with LangGraph
- Better retrieval techniques like Contextual Retrieval, ColBERT, and GraphRAG
- LLM testing and evaluation using Ragas and DeepEval
- Improving LLM security and handling prompt injection
- Making AI applications faster and cheaper to run

---

<p align="center">
  <em>Building projects, learning new things, and figuring out how to make them better.</em>
</p>