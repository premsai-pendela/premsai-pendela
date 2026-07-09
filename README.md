# 👋 Hi, I'm Naga Prem Sai Pendela

**Applied AI & Data Solutions Engineer**

I build **governed, role-aware AI systems** over SQL and documents — the kind where the hard part isn't getting an LLM to answer, it's making sure it only answers with what it's allowed to know, and can prove its work.

---

## 🚀 Featured Project

[![NexusIQ AI Platform](https://img.shields.io/badge/GitHub-NexusIQAI_Platform-24292e?style=for-the-badge&logo=github)](https://github.com/premsai-pendela/NexusIQAI-Platform)
[![Live Demo](https://img.shields.io/badge/Live_Demo-nexusiq--ai.com-success?style=for-the-badge)](https://nexusiq-ai.com/platform)

### NexusIQ AI Platform — Governed Multi-Company AI Data Analyst

> *Employees log in to their company's workspace and ask questions in plain English. Answers carry SQL, citations, a chart, an access decision, and a reviewable trace.*

Each company gets its own SQL schema and document "brain." Role-based access is enforced at **four independent layers** — SQL prompt scoping, `sqlglot` AST table allowlists, ChromaDB metadata filters, and response-level citation checks — so a request can never widen what it's allowed to see.

### What Makes It Different

| Capability | Details |
|---|---|
| **Role-scoped access** | 4-layer enforcement baked into the agent instance, not a request filter |
| **Deterministic analyst layer** | 15 business-metric families answered with **zero LLM calls** |
| **Session memory** | Multi-turn follow-ups resolve deterministically; re-authorized every turn |
| **Admin Health Check Agent** | Manually-triggered trace audit that proposes fixes, gated by human verification |
| **Full audit loop** | Per-employee traces, company-scoped feedback review, trace-leakage auditing |

### Scale & Stack

- **3 synthetic companies**, 35-table schema each, on **AWS RDS Postgres**
- **347+ tests**: AST denial, RAG boundary, cross-company memory isolation
- Deployed on **AWS ECS Fargate**, behind an **ALB with ACM-issued HTTPS**, frontend on **AWS Amplify**
- Model gateway across **Gemini, Groq, NVIDIA NIM, AWS Bedrock**, and local Ollama fallback

`Python` `FastAPI` `LangGraph` `Next.js` `TypeScript` `PostgreSQL` `ChromaDB` `sqlglot` `AWS (ECS, RDS, Bedrock, ALB)` `Docker`

---

## 📁 Other Projects

### RevenueIQ AI — Business Analytics & ML Platform

[![Live Demo](https://img.shields.io/badge/Live_Demo-RevenueIQ_AI-success?style=for-the-badge)](https://revenueiq-ai-9cnn.onrender.com)

Processed **534K+ public UCI retail transactions** into business-ready analytics across **$10.6M analyzed revenue** and **4,339 customers**.

- Built **5 ML/analytics workflows**: 95% F1 churn prediction, K-Means segmentation, Isolation Forest anomaly detection, ARIMA/ETS forecasting — identified **978 at-risk customers**
- Accelerated SQL analytics **7.7×** by replacing Pandas paths with DuckDB
- Automated executive reports with Groq LLM — cut report generation from **2 hours to 60 seconds**

`Python` `SQL` `DuckDB` `Scikit-learn` `Streamlit` `Plotly` `Groq LLM`

➡️ https://github.com/premsai-pendela/revenueiq-ai

---

## 🛠 Technical Skills

**AI/LLM Engineering**: Multi-agent orchestration (LangGraph) · RAG (hybrid BM25 + vector, cross-encoder reranking) · role-based access control for LLM systems · deterministic answer routing · Gemini · Groq · NVIDIA NIM · AWS Bedrock

**Reliability & Evals**: LLM evals, golden tests, retrieval benchmarks, evidence gating, SQL AST validation (`sqlglot`), trace logging/audit, cost-aware model routing

**Languages & Backend**: Python · SQL · TypeScript · FastAPI · Next.js/React · REST APIs

**Data & Cloud**: PostgreSQL (AWS RDS) · SQLAlchemy · ChromaDB · DuckDB · AWS (ECS Fargate, ALB/ACM, RDS, Bedrock, Secrets Manager, CloudWatch, ECR) · AWS Amplify · Docker

**Machine Learning**: Scikit-learn · Time series forecasting · Customer segmentation · Churn prediction

---

## 🎯 Current Focus

- Building **governed, multi-tenant AI systems** where access control is structural, not prompt-based
- Designing **deterministic-first analytics** so products stay reliable when LLM providers rate-limit
- Deepening AWS cloud deployment experience — ECS, RDS, Bedrock, IAM-scoped infrastructure

---

## 📫 Connect With Me

📧 nagapremsaip07@gmail.com
💼 https://www.linkedin.com/in/nagapremsai-pendela/
💻 https://github.com/premsai-pendela

---

⭐ Open to **Applied AI Engineer / AI Data Solutions Engineer** roles — feel free to reach out.
<!---
premsai-pendela/premsai-pendela is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
