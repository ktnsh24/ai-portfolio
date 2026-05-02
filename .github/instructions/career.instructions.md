# career.instructions.md — Career & Resume Tracker

> **Type:** Dimension table (current state, always up-to-date)
> Last updated: 2026-05-01

---

## Ketan's Profile

- **Current role:** Data & ML Platform Engineer @ Wipro (Client: Odido — Journey Team), The Hague
- **Start date at current role:** Feb 2026
- **Previous role:** Data & Analytics Engineer @ Wipro (Client: Odido — Mass Market B2C), Jul 2022 – Feb 2026
- **Location:** The Hague, Netherlands
- **Email:** ktnsh03@gmail.com | **Phone:** +31 6 4443 8329
- **LinkedIn:** `linkedin.com/in/ketan-sahu` ⚠️ **UNCONFIRMED — needs verification**
- **Total experience:** 6+ years in data engineering

---

## Active Application: ABN AMRO

### Role tracker

| # | Role title | JD focus | Resume file | Status |
|---|---|---|---|---|
| 1 | CDO Data Engineer | Metadata mgmt, lineage, governance; Databricks/Delta Lake/dbt | `personal/career/resumes/Ketan_resume_ABN.md` | ✅ On disk, edited 2026-05-01, **not yet committed** |
| 2 | (unknown) | Not discussed | Not created | ❌ Not started |
| 3 | F&R Platform DE | Financial Risk platform; likely Spark/Python/cloud | `personal/career/resumes/abn/Ketan_resume_ABN_role3.md` | ⚠️ Drafted in chat — **NOT saved to disk** |
| 4 | Senior DE — Credit Risk Services | Credit risk data pipelines; Azure prominent in JD | `personal/career/resumes/abn/Ketan_resume_ABN_role4.md` | ⚠️ Drafted in chat — **NOT saved to disk** |

### Motivation letter tracker

| Role | File | Status |
|---|---|---|
| Role 4 — Credit Risk Services | `personal/career/resumes/abn/motivation_letter_role4.md` | ⚠️ Drafted in chat — **NOT saved to disk** |

### Motivation letter — Role 4 structure (for recovery from chat if needed)

- **Salutation:** Dear Hiring Team
- **Para 1:** Why banking / ABN AMRO / AI angle — data quality as the foundation for risk decisions
- **Para 2:** Current ML platform work at Odido Journey team — real-time NBA, Medallion Architecture, Delta Lake, Databricks, Terraform IaC
- **Para 3:** Gen AI / Agentic AI hands-on — ai-portfolio repos (RAG chatbot, MCP server, multi-agent) demonstrating proactive learning beyond the day job
- **Para 4:** Engineering craft + honest Azure framing — AVEVA (Synapse, ADF), ADF patterns at Odido, Azure Key Vault equivalents; not inflating Azure depth
- **Paste instruction:** Strip lines 1–2 (markdown heading + blank line) before pasting into portal

---

## Known Open Threads

| Thread | Detail | Priority |
|---|---|---|
| Save unsaved files | Role 3 resume, Role 4 resume, motivation letter exist only as chat output | 🔴 High — do first |
| `abn/` folder creation | Folder `personal/career/resumes/abn/` doesn't exist yet | 🔴 Blocking file saves |
| LinkedIn handle verification | `linkedin.com/in/ketan-sahu` — confirm this is correct | 🟡 Medium — before submitting |
| Azure DevOps ATS gap (Role 4) | JD lists Azure DevOps; user removed it from resume; potential ATS filter miss | 🟡 Medium — worth a single line in skills |
| ThoughtSpot in Role 1 | Not in CDO JD; minor noise | 🟢 Low — cosmetic |
| Role 2 resume | Never discussed; unclear if needed | 🟢 Low — confirm with Ketan |
| Commit all ABN resume files | Role 1 modified but not committed | 🟡 Medium |

---

## Working Rules (from `.github/copilot-instructions.md`)

- **No PDF generation** unless explicitly requested
- **No table formatting in resumes** — use plain text, bold labels, or bullets only
- **Advisor behaviour:** challenge bad decisions, state trade-offs, hold positions under pressure
- Disagreement is not disrespect — best outcome > comfortable conversation

---

## Resume — Core Skills Reference (Ketan's actual stack)

**Strong (production experience):**
- Databricks (PySpark), Delta Lake, Delta Live Tables, dbt, Medallion Architecture
- AWS (S3, Glue, Redshift, Step Functions, Secrets Manager, Lake Formation, IAM)
- Terraform (reusable modules), GitHub Actions CI/CD
- Python (PySpark, Pydantic, boto3), SQL, Shell

**Moderate (production but limited depth):**
- Azure Data Factory, Azure Synapse Analytics (AVEVA + Odido patterns)
- Azure Key Vault (equivalent patterns to AWS Secrets Manager)
- Azure DevOps (CI/CD, used at Odido)
- Apache Airflow (Brainbay)

**Portfolio / learning (not production):**
- LangChain, LangGraph, OpenAI API, MCP protocol, RAG pipelines
- FastAPI, Docker, Pydantic v2

**Do not claim:**
- Deep Azure architecture design (honest: user-level, not architect-level)
- Spark performance tuning at scale (standard patterns only)

---

## Files in `personal/career/resumes/`

```
personal/career/resumes/
├── Ketan_resume_ABN.md           ← Role 1 (CDO DE) — on disk ✅
├── Ketan_resume-AI-Augmented-DE.md ← General AI-augmented DE resume — on disk ✅
└── abn/                          ← ⚠️ FOLDER DOES NOT EXIST YET
    ├── Ketan_resume_ABN.md       ← Role 1 copy (future — move here for consistency)
    ├── Ketan_resume_ABN_role3.md ← Role 3 (F&R Platform) — chat only ❌
    ├── Ketan_resume_ABN_role4.md ← Role 4 (Credit Risk Services) — chat only ❌
    └── motivation_letter_role4.md ← Motivation letter — chat only ❌
```
