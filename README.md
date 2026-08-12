<div align="center">

<img src="assets/header.svg" alt="Shresth Modi — AI/ML engineer, Bengaluru. Retrieval-augmented generation, LLM agents, and machine learning that ends in a decision." width="100%">

<br><br>

[![Email](https://img.shields.io/badge/Email-3B322B?style=flat-square)](mailto:meshrsth10@gmail.com)
[![MutualMind](https://img.shields.io/badge/MutualMind_·_live-3B322B?style=flat-square)](https://mutualmind.onrender.com)
[![Retention engine](https://img.shields.io/badge/Retention_engine_·_live-3B322B?style=flat-square)](https://decision-driven-customer-retention.streamlit.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-3B322B?style=flat-square)](https://www.linkedin.com/in/shresth-modi-793095293/)

</div>

<br>

> I build machine learning systems that end in a **decision**, not a dashboard.

Most of my work sits one layer above the model. A churn probability is worth nothing until it becomes a budget-constrained action with a number attached. A chatbot answer is worth nothing until it's grounded in something you can point at. That gap is the interesting part, and it's what both of my main projects are really about.

I'm in my final year, looking for **AI/ML and data science roles** — open to software engineering and full-stack too. Away from the keyboard: football, fashion, and a mutual-fund habit I got tired of tracking in spreadsheets, which is how MutualMind started.

<br>

## Highlights

| | |
|:--|:--|
| **Research** | Paper on OWASP Juice Shop for cybersecurity education — **accepted for publication**. Maps vulnerabilities to learning outcomes across 10+ attack categories. |
| **Industry** | **AI Engineering Intern, Wipro (Harman)** — Feb–Jun 2026. Multimodal RL-RAG retrieval, and an automated multi-agent crash-log triage pipeline. |
| **Shipped** | **MutualMind** — live in production. ~19.7K LOC, 52 REST endpoints, 83 automated tests. |
| **Leadership** | **Vice President, Aegis** — the cybersecurity and ethical hacking club at RVITM. Ran hands-on web-security workshops. |
| **Academics** | B.E. Information Science & Engineering, RVITM. **CGPA 8.54.** 2023–2027. |

<br>

## What I work with

| | |
|:--|:--|
| **Languages** | Python, Java, C, C++, SQL |
| **Machine learning** | scikit-learn, pandas, NumPy, SciPy, SHAP, Optuna, lifelines, PuLP |
| **LLM systems** | RAG, vectorless retrieval, LangChain, LangGraph, LLM agents, Azure OpenAI, Google Gemini, MCP, evaluation |
| **Backend and data** | FastAPI, Flask, Node/Express, MongoDB, PostgreSQL, SQLite, Redis, BigQuery, JWT/OAuth |
| **Interface** | React, Streamlit, Recharts, Plotly |
| **Tooling** | Git, Docker, GitHub Actions, pytest, Jest, ruff, mypy |

<br>

## Selected work

### MutualMind — an AI mutual-fund advisor

**[Repository](https://github.com/shrsth/mutualmind)** · **[Live](https://mutualmind.onrender.com)** · React 19, Node/Express 5, MongoDB Atlas, Google Gemini

A full-stack advisory platform for Indian mutual-fund investors that computes its analytics rather than just displaying them, and answers financial questions through a **vectorless RAG** chatbot — two-hop LLM tree-navigation across a 39-section knowledge base, with no embeddings and no vector database. It exists because the ungrounded model confidently returned a wrong LTCG rate. Grounded, it answers correctly.

| | |
|:--|:--|
| Scale | ~19.7K LOC · 52 REST endpoints · 21 pages · 8 portfolio-analytics tabs |
| Financial core | XIRR by Newton-Raphson (1e-6 tolerance) · 500-run Monte Carlo goal simulation · STCG/LTCG engine with FIFO accounting and the ₹1.25L exemption |
| Testing | 83 automated Jest tests across 4 suites |
| Security | Closed a JWT-forgery hole with boot-time secret validation · remediated **16 → 3** dependency CVEs |

*Demo account: `demo@mutualmind.dev` / `demo12345`. Render's free tier takes about 50 seconds to wake on the first request.*

<br>

### Decision-Driven Customer Retention

**[Repository](https://github.com/shrsth/decision-driven-customer-retention)** · **[Live](https://decision-driven-customer-retention.streamlit.app/)** · Python, scikit-learn, lifelines, PuLP, FastAPI, Docker

An end-to-end decision system over 7,043 real telecom customers that turns calibrated churn probabilities into budget-constrained ACT / MONITOR / IGNORE actions, then validates those decisions before deployment. Logistic Regression won a five-fold bake-off against gradient boosting on both discrimination *and* calibration — so the simpler model was kept on evidence rather than preference.

| | |
|:--|:--|
| Model | ROC AUC **0.845** (5-fold CV, ±0.013) · Brier **0.136** · calibrated across all ten deciles |
| Decisions | $25K budget → 261 customers targeted, ~$88.5K expected net value, **3.54× ROI** |
| Optimization | Greedy selection measured against an exact ILP 0-1 knapsack — captures ~**100%** of the optimum |
| Causal | T-learner uplift on a 64K-customer A/B test — Qini **1083 vs 148**, roughly 7× more incremental responders |
| Engineering | 51 pytest tests · GitHub Actions running ruff, mypy and coverage |

*The economics rest on a derived CLV and a stated 30% intervention-success assumption. The project quantifies its own break-even rather than hiding it.*

<br>

### Zero-Trust Dropbox

**[Repository](https://github.com/shrsth/zero-trust-dropbox)** · Python, Flask, Tkinter, TOTP, public-key cryptography

A secure file vault that verifies identity, device and context on every action instead of trusting network location. Multi-factor authentication pairing a password with a time-based one-time code; device identity attestation through a cryptographic key pair, so only registered devices are admitted; geolocation policy enforcement by IP; client-side encryption and time-limited access grants.

<br>

### AI Engineering Intern — Wipro (Harman)

February to June 2026 · RAG, multi-agent systems, Docling, spaCy, Azure OpenAI, BigQuery

*Client work, described at architecture level only.*

**Multimodal RL-RAG platform.** Built the primary and fallback document-processing pipelines, structuring content into hierarchical parent–child chunks so broad context stays linked to fine-grained retrieval units, with fallback handling for documents that failed primary extraction. Contributed to benchmark testing across text and image-grounded content.

**Log triaging agent.** Built a fully automated multi-agent pipeline for mobile crash logs — a continuous poller, a parser that extracts structured evidence, a root-cause classifier, and a severity and priority decision engine, all under a central coordinator — closing the loop to automated ticket creation through an agent-to-agent handoff.

<br>

---

<div align="center">

**Open to AI/ML, data science and software engineering roles.**

[meshrsth10@gmail.com](mailto:meshrsth10@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/shresth-modi-793095293/) &nbsp;·&nbsp; [Try MutualMind](https://mutualmind.onrender.com)

<br>

<sub>Every number here is drawn from the codebase it describes.</sub>

</div>
