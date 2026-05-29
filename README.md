# 👋 Hi, I'm Naga Prem Sai Pendela

**AI Engineer | Applied AI Engineer | Multi-Agent Systems**

![](https://komarev.com/ghpvc/?username=premsai-pendela&color=blueviolet&style=plastic)

I build **production-grade AI systems** that turn real-world data into intelligent, decision-ready insights — using multi-agent orchestration, LLMs, hybrid RAG, and machine learning — deployed on real infrastructure.

---

## 🚀 Featured Project

[![NexusIQ AI](https://img.shields.io/badge/Live_Demo-NexusIQ_AI-blueviolet?style=for-the-badge)](https://nexusiq-ai.com)
[![GitHub](https://img.shields.io/badge/GitHub-NexusIQ_AI-black?style=for-the-badge&logo=github)](https://github.com/premsai-pendela/NexusIQ-AI)

## NexusIQ AI — Production 4-Agent Business Intelligence Platform

> *Ask a business question in plain English. Get a cited, confidence-scored answer validated across SQL, documents, and live web data — in 5–12 seconds.*

An enterprise-grade **multi-agent AI platform** deployed on **AWS EC2** that routes natural language questions through a coordinated network of specialized agents — then cross-validates results across sources before returning a single trusted answer.

### Architecture

```
User Question
      │
Query Router  (Gemini 2.5 Flash — smart routing to sql/rag/web/all)
      │
      ├──────────────┬──────────────────┐
      ▼              ▼                  ▼
  SQL Agent      RAG Agent          Web Agent
 (90K rows       (43 PDFs           (5 product
  Supabase)       ChromaDB)          categories
                  BM25 + vector      4 scrapers)
      │              │                  │
      └──────────────┴──────────────────┘
                     │
              Fusion Agent
    Cross-validates SQL ↔ PDF numbers (< 1% = HIGH confidence)
    Deterministic formatting for validated facts (no LLM call)
    LLM synthesis only for conflicts or low confidence
                     │
         Cited answer · Confidence badge · Trace ID
```

### Screenshots

| Home | Multi-Agent Fusion |
|---|---|
| ![Home](https://raw.githubusercontent.com/premsai-pendela/NexusIQ-AI/main/Screenshots/home.png) | ![Multi-Agent](https://raw.githubusercontent.com/premsai-pendela/NexusIQ-AI/main/Screenshots/mutli-agent.png) |

| SQL Agent | Auto Chart |
|---|---|
| ![SQL](https://raw.githubusercontent.com/premsai-pendela/NexusIQ-AI/main/Screenshots/chat-sql.png) | ![Chart](https://raw.githubusercontent.com/premsai-pendela/NexusIQ-AI/main/Screenshots/chart.png) |

### What Makes It Different

| Capability | Details |
|---|---|
| **SQL Agent** | Natural language → SQL → Interactive Plotly charts on 90K rows · Supabase PostgreSQL |
| **RAG Agent** | Hybrid BM25 + vector search + cross-encoder reranker · **97.7% Hit@5**, 0.919 Context Recall |
| **Cross-Validation** | SQL ↔ PDF numbers reconciled to **0.03% delta** — HIGH confidence without manual fact-checking |
| **Fusion Agent** | Orchestrates all agents · deterministic formatting for validated facts · confidence badges |
| **Web Agent** | Live competitor pricing via Selenium + BeautifulSoup + Shopify API · 24hr TTL cache |
| **Fault Tolerance** | Circuit breaker: Gemini 2.5 Flash → Groq LLaMA 3.3-70B automatic fallback |
| **Observability** | Every query traced to AWS CloudWatch + local JSONL ledger · LLM gateway telemetry |

### Scale & Production

- **90,500 sales transactions · $175.6M revenue** across 5 regions and 5 product categories
- **43 business PDFs** across 8 categories — 425 ChromaDB chunks · all grounded in live Supabase data
- **Dual-LLM**: Gemini 2.5 Flash (primary) + Groq LLaMA 3.3-70B (fallback) with circuit breaker
- **Parallel execution** via `ThreadPoolExecutor` — ~60% latency reduction vs. sequential agents
- **Test coverage**: 97 unit tests · 12 golden eval cases · 7 offline evals · 43-query RAG benchmark
- **Deployed**: AWS EC2 (`t3.small`) · Docker · ECR · S3 · Secrets Manager · CloudWatch · GitHub Actions CI/CD · Caddy HTTPS · custom domain

`Python` `LangGraph` `Streamlit` `Google Gemini` `Groq` `PostgreSQL/Supabase` `ChromaDB` `BM25` `AWS EC2` `Docker` `GitHub Actions`

---

## 📁 Other Projects

### RevenueIQ AI — ML-Powered Business Intelligence Platform

[![Live Demo](https://img.shields.io/badge/Live_Demo-RevenueIQ_AI-34d399?style=for-the-badge)](https://revenueiq-ai-9cnn.onrender.com)
[![GitHub](https://img.shields.io/badge/GitHub-RevenueIQ_AI-black?style=for-the-badge&logo=github)](https://github.com/premsai-pendela/revenueiq-ai)

ML-powered analytics platform that analyzed **534K retail transactions ($10.6M revenue)** and surfaced **$4M+ in actionable business opportunities**.

| Model | Result |
|---|---|
| Random Forest churn prediction | **95% F1-score** · 978 at-risk customers flagged |
| KMeans segmentation (k=5) | 18 VIP Champions ($96K avg each) · 1,692 Potential Growers |
| Isolation Forest anomaly detection | 5,249 anomalies — identified as B2B/wholesale, not fraud |
| Prophet + ARIMA/ETS forecasting | $1.61M 30-day forecast · 9% MAPE (91% accuracy) |
| Groq LLM executive reports | 2 hours → **60 seconds** report generation |

- **7.74× faster queries** via DuckDB over Pandas — dashboard reload 45s → ~3s
- ML results stored as **DuckDB tables** — queryable by the whole team via SQL, not locked in Python
- Deployed on Streamlit Cloud + Render · UptimeRobot keep-alive

`Python` `Scikit-learn` `DuckDB` `SQL` `Groq LLaMA 3.3-70B` `Plotly` `Streamlit` `Pandas` `Prophet`

---

## 📄 Publication

**IEEE ADICS 2024** — [Enhancing Cyberbullying Detection Using Machine Learning](https://ieeexplore.ieee.org/document/10533585)

Built and validated a **47,000-instance NLP dataset** for cyberbullying detection. Led data pipeline: text normalisation, deduplication, label validation, feature engineering. Comparative evaluation of SVC, MNB, and GloVe-based pipelines — **79.8% classification accuracy**. Published peer-reviewed methodology at IEEE ADICS 2024.

---

## 🛠 Technical Skills

### AI & LLM Engineering
Multi-Agent Orchestration · LangGraph · RAG Pipelines · Hybrid BM25 + Vector Search
Cross-Encoder Reranking · LLM Routing & Fallback · Prompt Engineering
Google Gemini · Groq · ChromaDB · HuggingFace Embeddings

### Languages & Data
Python · SQL · Pandas · NumPy · Feature Engineering · Exploratory Data Analysis

### Machine Learning
Scikit-learn · Random Forest · KMeans · Isolation Forest · Prophet · ARIMA/ETS
Time Series Forecasting · Customer Segmentation · Churn Prediction · Anomaly Detection

### Databases
PostgreSQL · Supabase · DuckDB · ChromaDB · SQLAlchemy · Vector Databases

### Cloud & DevOps
AWS EC2 · AWS ECR · AWS S3 · AWS Secrets Manager · CloudWatch
Docker · GitHub Actions · CI/CD · Caddy · HTTPS

### Visualization & BI
Plotly · Streamlit · Plotly Dash · Matplotlib

---

## 🎯 Currently Targeting

- **AI Engineer** and **Applied AI Engineer** roles at companies shipping production AI
- **Forward Deployed Engineer (FDE)** roles at AI-first companies (Anthropic, OpenAI, Scale AI)
- Open to roles involving multi-agent systems, LLM engineering, RAG pipelines, and cloud-deployed AI

---

## 📫 Connect

📧 nagapremsaip07@gmail.com
💼 [linkedin.com/in/nagapremsai-pendela](https://www.linkedin.com/in/nagapremsai-pendela/)
🌐 [premsai-pendela.github.io](https://premsai-pendela.github.io)

---

⭐ Open to collaborating on **production AI systems, multi-agent orchestration, and LLM engineering** — feel free to reach out.

<!---
premsai-pendela/premsai-pendela is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
