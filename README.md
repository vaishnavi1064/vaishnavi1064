<p align="center">
  <a href="https://github.com/vaishnavi1064">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=100&lines=Vaishnavi+Chaughule;AI%2FML+Engineer+%C2%B7+Multi-Agent+Systems+%C2%B7+Research" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <strong>M.S. Computer Science @ Northeastern University, Seattle (Khoury College) · GPA: 3.67</strong>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/vaishnavichaughule"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:vaishnavi10chaughule@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/vaishnavi1064"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" /></a>
</p>

---

I build **research-grounded AI agent systems** and ship them to production. My work sits at the intersection of multi-agent orchestration, vector retrieval, and ML evaluation — grounded in peer-reviewed literature (EMNLP, NAACL, ACL, ICSE, MSR), not just API wrappers.

Currently conducting **faculty-supervised research** at Northeastern on **Cross-Modal Semantic Drift** detection in generative AI, with two Stanford University co-mentors — extending Microsoft Research's Argos agentic verifier framework and targeting publication.

**Open to Summer / Fall 2026 internships** in AI/ML Engineering, SDE, or Applied Research.

---

## What I Build With

**AI/ML & Agent Systems:**
`Groq (Llama 3.3 70B)` `Jina Embeddings` `Hugging Face / sentence-transformers` `ChromaDB` `FAISS` `Scikit-learn` `Pydantic v2` `MCP (Model Context Protocol)` `RAG Pipelines` `AsyncIO`

**Full-Stack & Backend:**
`Python` `Java` `TypeScript` `JavaScript` `SQL` `Kotlin` `FastAPI` `React` `Node.js` `Express` `Django` `Flask`

**Infrastructure & Data:**
`AWS (EC2, RDS, ALB, Auto Scaling)` `Supabase` `PostgreSQL` `MySQL` `Docker` `GitHub Actions` `Vercel` `Render` `Linux/Bash`

---

## Featured Projects

### PersonaCR — Research-Grounded Multi-Agent Code Review System
**`FastAPI` `React` `TypeScript` `Groq` `Jina Embeddings` `ChromaDB` `Supabase` `MCP`** · [Repo](https://github.com/vaishnavi1064/PersonaCR)

A 6-agent code review system that learns a developer's **personal coding fingerprint** and reviews new code against their own patterns — not generic rules. Research-grounded in 9 peer-reviewed papers across EMNLP 2024, NAACL 2025, ACL 2024, and MSR 2026.

- **Multi-agent orchestrator** with parallel execution via `asyncio.gather` (Style Analyst + Defect Hunter) — ~48% latency savings, ~6.1s total
- **Two autonomous loops:** confidence-based re-planner + CRScore-inspired quality gate using `all-MiniLM-L6-v2` semantic similarity scoring (~69ms after warmup)
- **Code fingerprinting pipeline:** Jina embeddings (768-dim, 30 languages) in ChromaDB with metadata-filtered retrieval across multi-repo codebases
- **ML evaluation layer (Layer 3):** Pseudo-reference generation (AST + Groq LLM hybrid), STS scoring, rules-based quality gate — adds ~1.1s overhead
- **MCP server** via `fastapi-mcp`, exposing `analyze_repo`, `review_code`, `health_check` to Claude Code, Cursor, and VS Code
- **Full-stack:** React + TypeScript frontend, Supabase PostgreSQL with GitHub OAuth, cross-session persistence
- **End-to-end pipeline latency:** ~8.5 seconds

<details>
<summary><strong>Research foundation (9 papers)</strong></summary>

| Paper | Venue | What it informed |
|-------|-------|------------------|
| CodeAgent | EMNLP 2024 | Multi-agent code review architecture |
| CRScore | NAACL 2025 | ML evaluation pipeline & quality gate |
| MPCODER | ACL 2024 | Personalized code style learning |
| RevAgent | 2025 | Agent-based review orchestration |
| Latency-Aware MAS | 2026 | Parallel execution design |
| Multi-Agent Design (Google) | 2025 | Agent coordination patterns |
| Ghaleb | MSR 2026 | Code review quality metrics |
| Ringer | 2025 | Review comprehensiveness scoring |
| Ericsson | 2025 | Industrial code review practices |

</details>

---

### Third-Place-Finder — AI Recommendation Engine
**`React` `TypeScript` `Node.js` `Express` `MySQL` `Groq (Llama 3.3 70B)` `Leaflet`** · [Repo](https://github.com/vaishnavi1064/Third-Place-Finder-Web) · [Live Demo](https://third-place-finder-web.vercel.app/)

A full-stack recommendation engine with a multi-stage RAG pipeline that maps natural language queries to structured categories, retrieves candidates via Geoapify API, and ranks top 10 with LLM-generated rationale. Features fault-tolerant LLM integration with exponential backoff, anti-hallucination prompting, and context engineering — deployed live across Vercel, Render, and Aiven.

---

### OULAD Concurrent Data Analytics Engine
**`Java` `Multithreading` `BlockingQueue` `ConcurrentHashMap` `JUnit 5`** · [Repo](https://github.com/vaishnavi1064/OULAD-Concurrent-Data-Analytics-Engine)

Scalable data pipeline processing **10.6M rows at 2.1M rows/second** using producer-consumer architecture with BlockingQueue, ConcurrentHashMap, and poison pill termination. Achieved **94% instruction and 88% branch coverage** with 51 JUnit 5 tests including multi-threaded race condition harnesses across a 3-person team.

---

### Forest Fire Prediction
**`Python` `Scikit-learn` `Django`** · [Repo](https://github.com/vaishnavi1064/Forest-Fire-prediction)

Wildfire risk prediction using 36,000+ satellite and meteorological records. Improved R² from 0.65 to 0.68 using RandomizedSearchCV (50 iterations, 3-fold CV). Deployed via Django with model size reduced from 700MB to 93MB for real-time inference.

---

### Air Quality Prediction
**`Python` `Pandas` `Scikit-learn`** · [Repo](https://github.com/vaishnavi1064/Air-Quality-prediction)

AQI forecasting system using 435,000+ environmental records with engineered pollutant sub-indices (SO₂, NO₂, RSPM, SPM). Random Forest regression with cross-validation — R² > 0.99, RMSE of 1.15.

---

## Research

**Cross-Modal Semantic Drift Detection in Generative AI** · *In Progress*
Faculty-supervised research at Northeastern University with two Stanford University co-mentors. Extending Microsoft Research's Argos agentic verifier to detect and quantify semantic drift across modalities in generative AI outputs. Targeting publication.

---

## Experience

**IBM SkillsBuild** · AI & Machine Learning Intern · Jun – Jul 2024
Built supervised ML models for healthcare risk prediction, integrated into a chatbot. Developed IBM Cognos dashboards for KPI tracking.

**Google for Developers (AICTE)** · Android Development Intern · Jul – Sep 2024
Developed Android applications using Kotlin + MVVM architecture with SQLite local storage and REST API integration.

---

## Leadership

- **Program Manager** — GameCube Club, Northeastern University *(Sept 2025 – Present)*
- **Cloud Computing Lead** — Google Developer Groups *(Aug 2024 – Jul 2025)*
- **Event Co-Lead** — Google Developers Student Club *(Aug 2023 – Jul 2024)*

---

## Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vaishnavi1064/vaishnavi1064/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/vaishnavi1064/vaishnavi1064/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/vaishnavi1064/vaishnavi1064/output/github-snake.svg" />
</picture>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=vaishnavi1064&theme=tokyo-night&hide_border=true&area=true" width="100%" />
</p>
