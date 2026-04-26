# Learning Journey — Data Engineer to AI Platform Engineer

> Why this portfolio exists, how it is structured, and what each project taught me.

## Table of Contents

- [The premise](#the-premise)
- [Why these five projects](#why-these-five-projects)
- [Mapping AI concepts to data engineering](#mapping-ai-concepts-to-data-engineering)
- [How I work through each repo](#how-i-work-through-each-repo)

---

## The premise

I am a Data Engineer with multiple years of experience in ETL, data pipelines, AWS, and Terraform. The transition into AI/ML platform engineering does not require throwing that away — it requires extending it. Every modern AI system is, structurally, a data system: ingest, transform, store, query, serve.

This portfolio proves that with code instead of slides.

---

## Why these five projects

The five projects cover the full surface area of an AI platform engineer's day-to-day work:

| Phase | What I had to learn that was new | What I already knew that transferred |
|-------|----------------------------------|--------------------------------------|
| 1 — RAG chatbot | Embeddings, vector search, prompt design, golden-dataset eval | FastAPI, Terraform, AWS, Pydantic, async I/O |
| 2 — AI gateway | LiteLLM provider abstraction, semantic caching, per-key rate limiting | Redis, PostgreSQL, API design, cost monitoring |
| 3 — AI agent | LangGraph state machines, MCP client, tool-use loops | State management, retries, observability |
| 4 — MCP server | Protocol design, Zod schemas, TypeScript ecosystem | API contract design, schema validation |
| 5 — Multi-agent capstone | Agent orchestration, role specialization, WebSocket UI | Distributed coordination, frontend basics |

The order is deliberate. Each phase introduces **one new concept** so that I can reason about it cleanly before adding the next layer.

---

## Mapping AI concepts to data engineering

This is the cheat sheet I wish I had when I started:

| AI concept | Data engineering parallel | Why the parallel works |
|------------|--------------------------|------------------------|
| Embedding | A row in an index | Both are "fingerprints" used to find related rows quickly |
| Vector store | A search index (OpenSearch, Elasticsearch) | Both store fingerprints + metadata and let you query by similarity |
| Chunking | Partitioning | Both split a big dataset into smaller, retrievable pieces |
| Ingestion pipeline | ETL | Same five steps: extract, clean, transform, store, validate |
| Prompt | A SQL query template | Both are parameterized text that produces a result from a backend |
| RAG | ETL + lookup + render | Ingest documents (ETL), retrieve top-k (lookup), render answer (template) |
| LLM | A stateless function | Same input → roughly same output (with temperature 0); call from any service |
| Golden dataset | A test fixture | Known inputs with known expected outputs |
| Evaluation metric | A data quality check | "Does the output match expectations?" — same problem |
| Token | A row size unit | Both are how the platform meters and bills you |
| Agent | A workflow / DAG | Both are: decide step → execute → check result → loop or finish |
| MCP server | A microservice | Same idea: a contract-first server that exposes a set of operations |
| Vector similarity (cosine) | Jaccard / Levenshtein over rows | All measure "how close are these two records?" |

---

## How I work through each repo

The workflow is the same in every repo:

1. **Plan first.** Write Jira-style stories (Analysis A1/A2/… → Development D1/D2/…) before any code.
2. **Build the smallest end-to-end slice.** API + one provider + one happy path. Get it running locally.
3. **Add observability before features.** OpenTelemetry, structured logs, request IDs — never debug blind.
4. **Document as I build.** Every concept gets a doc with a DE parallel and a 🚚 courier one-liner.
5. **Run hands-on labs.** Change one config (chunk size, top-k, temperature, …), re-run the same golden questions, record metrics in a table. Conclusions backed by numbers, not vibes.
6. **Containerize and Terraform from day one.** Local-first development that maps cleanly to AWS or Azure deployment.
7. **Push to GitHub only when the README and `docs/reading-order.md` are publish-ready.**

The result is that a recruiter can clone any repo, read the reading order, run `docker compose up`, and have a working system in minutes — without me being there.
