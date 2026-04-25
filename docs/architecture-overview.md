# Architecture Overview

> How the five projects in this portfolio fit together as one learning arc.

## Table of Contents

- [The big picture](#the-big-picture)
- [Phase-by-phase](#phase-by-phase)
- [Shared conventions across all repos](#shared-conventions-across-all-repos)
- [Tech stack at a glance](#tech-stack-at-a-glance)

---

## The big picture

Each project introduces **one new architectural pattern** while reusing the conventions of the previous one. By the end, you have built every piece of a modern AI platform — from a single RAG API to a multi-agent system with a frontend.

```
                              AI Portfolio — learning arc
                              ───────────────────────────

   Phase 1            Phase 2            Phase 3            Phase 4            Phase 5
 ┌──────────┐      ┌──────────┐      ┌──────────┐      ┌──────────┐      ┌─────────────┐
 │   RAG    │ ───▶ │ Gateway  │ ───▶ │  Agent   │ ───▶ │   MCP    │ ───▶ │ Multi-Agent │
 │  Chatbot │      │  (Proxy) │      │  + Tools │      │  Server  │      │   Capstone  │
 └──────────┘      └──────────┘      └──────────┘      └──────────┘      └─────────────┘
   one LLM,         many LLMs,         tools +           protocol-          orchestration
   one API          one API            reasoning         standard            + frontend
                                                         tool host
```

- **Phase 1 (rag-chatbot)** — the foundation. One model, one vector store, one API. Production-grade docs and labs.
- **Phase 2 (ai-gateway)** — abstract the model layer. Many providers behind one OpenAI-compatible interface, with caching, rate limits, cost tracking.
- **Phase 3 (ai-agent)** — give the LLM tools. LangGraph for reasoning, MCP client to talk to external tool servers.
- **Phase 4 (mcp-server)** — be a tool server yourself. TypeScript implementation of the Model Context Protocol.
- **Phase 5 (ai-multi-agent)** — capstone. Multiple specialized agents collaborate, with a Next.js frontend and WebSockets for live updates.

The bonus **knowledge-engine** repo sits alongside Phase 1 as a more advanced RAG variant (GraphRAG, multi-store, gap detection).

---

## Phase-by-phase

| # | Repo | What's new vs the previous phase | Production-grade aspects |
|---|------|----------------------------------|--------------------------|
| 1 | rag-chatbot | Embeddings, vector search, prompt templates, golden dataset evaluation | Multi-cloud (AWS + Azure + local), Terraform, OpenTelemetry, 16 measurable labs |
| 2 | ai-gateway | Provider abstraction, semantic cache, per-key rate limits, cost ledger | OpenAI-compatible API, Redis caching, PostgreSQL cost storage |
| 3 | ai-agent | Tool use, planning, agent loops, memory | LangGraph state machine, MCP client integration |
| 4 | mcp-server | Protocol implementation, schema validation | TypeScript, Zod schemas, MCP SDK, deployable as a stdio or HTTP server |
| 5 | ai-multi-agent | Multi-agent orchestration, role specialization, real-time UI | CrewAI for orchestration, Next.js frontend, WebSocket updates |

---

## Shared conventions across all repos

Every repo follows the same patterns so that once you understand one, you can navigate the others in minutes.

| Convention | Why it matters |
|------------|----------------|
| `docs/reading-order.md` as the entry point | Guided tour from "what does this do" to deep internals |
| `docs/ai-engineering/` for AI concepts | Mapped to data-engineering parallels (embeddings = index, chunking = partitioning, …) |
| `docs/architecture-and-design/` | System design + per-route deep dives |
| `docs/hands-on-labs/` | Every config knob has a measurable lab — change one variable, run the same questions, record the metrics |
| `🫏 Donkey` column on every table | A one-line everyday analogy for every concept — readable without prior AI knowledge |
| Pydantic Settings for all config | One `.env` file per environment, fully type-checked |
| Ruff for lint + format | Single tool, no debate |
| Docker + Terraform | Local-first development, cloud-deployable from day one |
| Golden dataset + reproducible eval | Before/after metrics for every change, not "feels better" |

---

## Tech stack at a glance

| Layer | Tools used across the portfolio |
|-------|---------------------------------|
| Language | Python 3.12 (repos 1–3, bonus), TypeScript (repo 4), Python + TS (repo 5) |
| Web framework | FastAPI (Python), MCP SDK (TS), Next.js (frontend) |
| LLM providers | AWS Bedrock (Claude), Azure OpenAI (GPT-4o), Ollama (local) |
| Vector stores | OpenSearch, Azure AI Search, ChromaDB, DynamoDB ($0 alternative), Neo4j (graph) |
| Storage | S3, Azure Blob, DynamoDB, Cosmos DB |
| Observability | OpenTelemetry, Prometheus, Loguru |
| IaC | Terraform (modular, separate state per environment) |
| CI/CD | GitHub Actions |
| Containers | Docker (multi-stage builds) |
| Eval | Custom golden-dataset framework + RAGAS-style metrics |
