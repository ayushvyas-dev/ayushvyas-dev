<h1 align="center">Hi, I'm Ayush Vyas 👋</h1>

<p align="center">
  <em>AI & LLM Systems Engineer · Building Production Agentic Architectures, RAG Pipelines & Guardrail Frameworks</em>
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
- 🤖 Specializing in **AI Engineering, Agentic Workflows, RAG Architectures & LLM Reliability**
- 🏗️ Building production-grade AI systems with **Python, LangGraph, FastAPI, pgvector & Next.js**
- 🧠 Deep focus on **stateful agent orchestration, hybrid vector search (pgvector & Pinecone), multi-layer guardrails & automated evaluation harnesses**
- 🛡️ Passionate about solving core production AI challenges: hallucination prevention, latency & cost optimization, prompt injection defense, and strict PII protection
- 🎯 Goal: Engineer high-reliability AI/LLM infrastructure and contribute to forward-thinking AI teams
- ⚡ I learn by building complex systems from first principles and stress-testing them under real workloads

---

## 🛠️ Tech Stack

- **Languages:** Python, SQL, TypeScript, JavaScript, C++
- **AI & LLM Engineering:** Retrieval-Augmented Generation (RAG), Agentic AI, LangGraph, LangChain, Embeddings, Hybrid Search, Prompt Engineering, LLM Guardrails
- **LLM Evaluation & APIs:** LLM Evaluation, Recall@k, MRR, Groq, Google Gemini
- **Backend & Databases:** FastAPI, REST APIs, Pydantic, PostgreSQL, Supabase, Pinecone, pgvector, Redis, MongoDB, Node.js
- **Tools & DevOps:** Docker, Git, GitHub Actions, pytest, Linux, Prometheus, OpenTelemetry

---

## 🚀 Projects

### 🤖 AI Customer Support Agent

> An enterprise-ready agentic email support platform orchestrating self-correcting RAG workflows, multi-layer guardrails, and real-time push webhooks.

Built with a focus on **agent state machine orchestration, hallucination prevention, defense-in-depth safety, and production resilience**.

- 🔄 **LangGraph State Machine**: Cyclic agent orchestration with document relevance grading, runtime query rewriting, and self-correcting output retry loops
- 📚 **pgvector Semantic Search**: Chunks policies into 768-dimensional embeddings in Supabase PostgreSQL with cosine similarity search and policy grounding checks
- 🛡️ **Multi-Layer AI Guardrails**: Ingress prompt injection interception, bidirectional PII masking (Luhn-validated payment cards, CVVs, credentials) without corrupting order IDs, and unauthorized commitment detection (refunds, discounts, callbacks)
- ⚡ **Heterogeneous Model Cascade**: Low-latency classification via Groq (`gpt-oss-120b`) combined with grounded synthesis on Google Gemini (`gemini-2.5-flash`) and fallback redundancy
- 📬 **Real-Time Push Ingestion**: Event-driven Google Cloud Pub/Sub push webhooks to FastAPI with idempotent message processing and automatic Gmail watch renewal
- 📊 **Benchmarked & Tested**: Backed by a 42-test automated unit suite (100% pass) and evaluated against a 100-scenario golden benchmark across 11 edge-case categories

**Stack:** Python · FastAPI · LangChain · LangGraph · Supabase pgvector · Groq · Google Gemini · GCP Pub/Sub · Next.js · Docker

**Links:**
[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://ai-customer-support-coral-eight.vercel.app)
[![API Docs](https://img.shields.io/badge/API_Docs-009688?style=flat&logo=fastapi&logoColor=white)](https://ai-customer-support-jp8w.onrender.com/docs)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/ai-customer-support)

---

### 🛡️ LLM Guard — AI Security & Reliability Middleware

> An API-first security, validation, and policy enforcement gateway designed to safeguard LLM applications and AI agents in production.

Built with a focus on **adversarial robustness, low-latency synchronous inspection, data privacy, and asynchronous AI verification**.

- 🚫 **Prompt Injection & Jailbreak Defense**: Real-time detection of instruction hierarchy overrides, system prompt exfiltration attempts, and adversarial jailbreak templates
- 🔒 **High-Throughput PII Redaction**: Deterministic rules and regex for Indian PAN, Aadhaar, credit cards, CVVs, passwords, IP addresses, and API credentials with zero-leak redaction
- 🧩 **Agent Tool-Call & Output Validation**: Intercepts and validates LLM tool invocations, parameter boundaries, and schema conformity before actions run
- ⚖️ **Risk Scoring & Policy Engine**: Multi-tier risk classification with automated `allow`, `flag`, or `block` decisions based on configurable sensitivity thresholds
- 📬 **Asynchronous Verification Jobs**: BullMQ and Redis task queues for background verification scans, deep claim validation, and audit analysis
- 📝 **Comprehensive Audit Logging**: Structured logging of prompts, scanner detections, risk scores, and latency metrics stored in PostgreSQL via Prisma

**Stack:** TypeScript · Node.js · Express · Groq · BullMQ · Redis · PostgreSQL · Prisma · Zod

**Links:**
[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://guardllm.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/llmguard)

---

### 🔍 IncidentIQ — Grounded Incident Investigation & Decision-Support

> An evidence-grounded incident investigation and operational decision-support platform that synthesizes root-cause hypotheses with exact quote citations.

Built with a focus on **hybrid search ranking, strict evidence citation, model resilience, and full-stack observability**.

- 🔎 **Hybrid Retrieval Engine**: Fuses PostgreSQL full-text search (lexical) with Pinecone dense semantic vector search via Reciprocal Rank Fusion (RRF)
- 📑 **Asynchronous Document Ingestion**: Ingests runbooks, incident postmortems, architecture diagrams, and PDFs with deterministic chunking via ARQ and Redis workers
- 📌 **Exact Quote Citation Verification**: Synthesizes structured root-cause hypotheses and safe, read-only diagnostic steps strictly verified against verbatim source text
- 🔄 **Resilient LLM Routing**: Primary generation via Groq with automated Gemini fallbacks, exponential backoff retries, and circuit breakers
- 📈 **Evaluation Harness**: Offline and online benchmarking across versioned validation/holdout splits computing `Recall@k`, `Hit Rate`, `MRR`, `nDCG`, quote support rate, and latency/token costs
- 🔭 **Production Observability**: Full observability stack with Prometheus exposition (`/metrics`), structured logs, and OpenTelemetry (OTel) distributed tracing hooks

**Stack:** Python · FastAPI · SQLAlchemy · Pinecone · NeonDB PostgreSQL · ARQ · Redis · OpenTelemetry · Prometheus · Next.js

**Links:**
[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat&logo=vercel&logoColor=white)](https://incidentiq-ai.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayushvyas-dev/incidentiq)

---

## 🎯 Currently Learning

- Advanced Multi-Agent Orchestration & Hierarchical Decision-Making
- Advanced Retrieval Strategies (Contextual Retrieval, ColBERT & GraphRAG)
- LLM Evaluation Frameworks (Ragas, DeepEval & red-teaming benchmarks)
- AI Safety, Prompt Injection Robustness & Alignment
- Distributed LLM Inference, Latency & Cost Optimization

---

<p align="center">
  <i>Building reliable AI systems, breaking things, understanding them from first principles, and getting better every day.</i>
</p>
