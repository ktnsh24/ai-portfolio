# Reading Order

> Recommended order for exploring this portfolio, by available time.

## Table of Contents

- [If you have 5 minutes](#if-you-have-5-minutes)
- [If you have 15 minutes](#if-you-have-15-minutes)
- [If you have 1 hour](#if-you-have-1-hour)
- [If you have an afternoon](#if-you-have-an-afternoon)
- [Shared Lab Guidance](#shared-lab-guidance)
- [Cross-repo conventions](#cross-repo-conventions)

---

## If you have 5 minutes

1. **[Architecture overview](./architecture-overview.md)** — one page, recruiter-friendly summary of all six projects.
2. **[Main README](../README.md)** — the projects table.
3. Open **[rag-chatbot](https://github.com/ktnsh24/rag-chatbot)** and read its top-level `README.md`.

---

## If you have 15 minutes

Everything above, plus:

1. **[Architecture overview](./architecture-overview.md)** — how the five projects fit together as one learning arc.
2. **[Learning journey](./learning-journey.md)** — the DE-to-AI transition framing.
3. In **rag-chatbot**, read `docs/architecture-and-design/architecture.md` for the system design.

---

## If you have 1 hour

Everything above, plus:

1. In **rag-chatbot**, follow `docs/reading-order.md` Levels 1–3:
   - Level 1 — what is RAG, what does this repo do
   - Level 2 — request flow, key components
   - Level 3 — per-route deep dives (`/v1/chat`, `/v1/documents`, …)
2. Skim one **hands-on lab** to see how I measure changes — e.g. `docs/hands-on-labs/lab-01-chunk-size.md`.
3. Run it locally:

   ```bash
   git clone https://github.com/ktnsh24/rag-chatbot
   cd rag-chatbot
   cp .env.example .env
   docker compose up -d
   curl http://localhost:8000/v1/health
   ```

---

## If you have an afternoon

Everything above, plus:

1. Read **rag-chatbot** `docs/reading-order.md` Levels 4–8 (cloud, infra, CI/CD, evaluation framework).
2. Open **ai-gateway** and read its `docs/ai-engineering/gateway-concepts.md` to see how the abstraction layer works on top of Phase 1.
3. Open **knowledge-engine** to see the GraphRAG variant — same conventions, different storage strategy.

---

## Shared Lab Guidance

Before diving into repo-specific labs, read the consolidated guide once:

- [Shared How to Read Labs](./shared/hands-on-labs/how-to-read-labs.md)

It defines the common lab pattern, default mode policy, and the one-panel comparison approach used across the portfolio.

Also use the shared AI-engineering baselines:

- [Shared Testing Playbook](./shared/ai-engineering/testing-playbook.md)
- [Shared Cost Analysis Playbook](./shared/ai-engineering/cost-analysis-playbook.md)

---

## Cross-repo conventions

Every repo in this portfolio follows the same structure, so once you have explored one you can navigate the others in minutes:

| Folder | Contents |
| --- | --- |
| `docs/reading-order.md` | Guided tour, ordered by depth |
| `docs/ai-engineering/` | AI concepts mapped to DE parallels |
| `docs/architecture-and-design/` | System design + per-route deep dives |
| `docs/setup-and-tooling/` | Local setup, Docker, Terraform, debugging |
| `docs/reference/` | API reference, Pydantic models, monitoring |
| `docs/hands-on-labs/` | Measurable experiments with before/after metrics |

Every doc table includes a 🚚 **Courier** column — a one-line everyday analogy. The convention is intentional: it forces every technical concept to also be explainable in plain English, which is the single best test for whether I actually understand it.
