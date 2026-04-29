# AI Portfolio

> **From Data Engineer to AI Platform Engineer — five production-grade AI systems built ground-up.**

This portfolio is a structured journey from data engineering into AI/ML platform engineering. Each repo demonstrates one architecture pattern, one tech stack, and a hands-on evaluation methodology (build → measure → improve → prove with data).

☁️ **Multi-cloud by design.** Every project ships with three deployment targets — **AWS** (Bedrock, OpenSearch, DynamoDB, ECS/Lambda), **Azure** (OpenAI, Cosmos DB, AI Search, Container Apps), and **local** (Docker Compose with open-source equivalents like ChromaDB, Neo4j, Postgres). The same code runs on all three; only the infra layer changes.

📄 For a recruiter-focused summary, see **[`docs/architecture-overview.md`](./docs/architecture-overview.md)** — one page covering all six projects, the learning arc, and how they fit together.

> 🖼️ **Architecture diagram coming soon** — a visual map of how the six projects compose into one platform across AWS, Azure, and local.

---

## The five projects

| # | Repo | Pattern | Stack | Status |
|---|------|---------|-------|--------|
| 1 | **[rag-chatbot](https://github.com/ktnsh24/rag-chatbot)** | Monolith RAG API | FastAPI · AWS Bedrock · Azure OpenAI · OpenSearch · ChromaDB | ✅ Core complete · 43 docs · 16 hands-on labs |
| 2 | **[ai-gateway](https://github.com/ktnsh24/ai-gateway)** | LLM Proxy / Gateway | LiteLLM · Redis · PostgreSQL | 🚧 In progress · 27 docs · 8 config-tuning labs |
| 3 | **ai-agent** | AI Agent with Tools | LangGraph · MCP Client · Tavily | 📋 Planned · 8 labs scaffolded |
| 4 | **mcp-server** | MCP Protocol Server | TypeScript · MCP SDK · Zod | 📋 Planned · 6 labs scaffolded |
| 5 | **ai-multi-agent** | Multi-Agent + Frontend (capstone) | CrewAI · Next.js · WebSockets | 📋 Planned · 14 labs scaffolded |
| ★ | **knowledge-engine** | Document RAG / Knowledge Base (bonus) | FastAPI · Neo4j · DynamoDB · Cosmos | 🚧 In progress · 31 docs · 19 labs scaffolded |

> Links above will go live as each repo is published. Start with **rag-chatbot** — it is the most complete and demonstrates the full RAG pipeline end to end.

---

## What recruiters should look at

If you have **5 minutes**:
1. Read [`docs/architecture-overview.md`](./docs/architecture-overview.md) — the 1-page summary of all six projects.
2. Open [rag-chatbot](https://github.com/ktnsh24/rag-chatbot) → `README.md` → architecture diagram.

If you have **15 minutes**:
1. Steps above, plus
2. Read [`docs/architecture-overview.md`](./docs/architecture-overview.md) — how the five projects fit together as one learning arc.
3. Skim [`docs/learning-journey.md`](./docs/learning-journey.md) — the DE-to-AI transition framing.

If you have **an hour**:
1. Steps above, plus
2. In `rag-chatbot`, read `docs/reading-order.md` and follow the recommended docs.
3. Run the chatbot locally — `docker compose up` and `curl localhost:8000/v1/chat`.

---

## Why this structure

Every repo follows the same documentation and quality conventions:

- **`docs/reading-order.md`** — a guided tour through the repo's docs, ordered by depth.
- **`docs/architecture-and-design/`** — system design + per-route deep dives.
- **`docs/ai-engineering/`** — AI concepts mapped to data engineering parallels.
- **`docs/setup-and-tooling/`** — local setup, Docker, Terraform, debugging.
- **`docs/reference/`** — API reference, Pydantic models, monitoring.
- **`docs/hands-on-labs/`** — measurable experiments (chunk size, top-k, temperature, …) with before/after metrics.

Every doc table includes a 🚚 **Courier** column — a one-line everyday analogy that makes complex AI concepts immediately readable.

---

## About me

I am a **Data Engineer** moving into **AI/ML platform engineering**. My background is ETL, data pipelines, AWS, Terraform, and Python. This portfolio is how I am proving the transition with code, not slides.

- **GitHub:** [ktnsh24](https://github.com/ktnsh24)
- **Cert targets:** AWS Generative AI Developer Pro (AIP-C01), Azure AI Engineer (AI-102)
- **Approach:** map every AI concept to a DE parallel, build production-grade APIs, measure everything with golden datasets

---

## License

[MIT](./LICENSE) — feel free to use any of this code or docs as a learning reference.
