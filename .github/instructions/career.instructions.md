# career.instructions.md — Career & Resume Tracker

> **Type:** Dimension table (current state, always up-to-date)
> Last updated: 2026-05-03

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

## Active Application: Netflix

### Role tracker

| # | Role title | JD focus | Resume file | Status |
|---|---|---|---|---|
| 1 | Senior Analytics Engineer | Legal org / Content Enterprise DS&E; KPI ownership, metric design, stakeholder translation; Claude Code in JD | `personal/career/resumes/Ketan_resume_Netflix_AE.md` | ⚠️ Drafted in chat — **NOT saved to disk** |

### Motivation letter tracker

| Role | File | Status |
|---|---|---|
| Senior Analytics Engineer | `personal/career/resumes/motivation_letter_netflix.md` | ⚠️ Drafted in chat — **NOT saved to disk** |

### Netflix resume — key framing decisions

- **Analytics-forward** (not DE-forward): KPI ownership, metric design, data storytelling, stakeholder translation
- **Claude Code named explicitly** — matches JD requirement; listed in AI Portfolio section
- **No Tableau** — honest gap; Power BI is the parallel tool; Streamlit noted in portfolio context
- **Experience framing:** "6+" years (JD asks 7 — slight gap, not a blocker)
- **CET timezone** noted naturally in summary (remote-friendly role signal)
- **AI Portfolio section:** bullet format, no tables

### Netflix motivation letter structure (for recovery from chat if needed)

- **Para 1:** Why Netflix / AI workflow angle — measurement at Netflix scale, AI-augmented analyst workflows
- **Para 2:** Odido domain ownership + anonymous stakeholder quote from recommendation letter ("one of my key business stakeholders")
- **Para 3:** AI portfolio specifics — RAG with 13 eval labs, LangGraph, MCP, CrewAI; shows proactive learning
- **Para 4:** CET timezone + measurement integrity framing — available for US West hours overlap; rigor over vanity metrics
- **American English** throughout
- **Paste instruction:** Strip header line (markdown `# …` line) before pasting into portal

### Netflix recommendation letter

- **File:** `personal/career/Letter of recommendation.md`
- **Author:** Jeremy Boeijink, Channel Manager, Commercial Management, Odido (business stakeholder, not tech manager)
- **Strength:** validates analytical credibility and stakeholder partnership from a business POV — strong fit for Analytics Engineer role
- **Name usage:** Jeremy's name removed from motivation letter; quote used anonymously; name is in the letter itself
- **Strategy:** submit as additional document in Netflix portal; resurface at interview stage
- **Jeremy confirmed** aware the letter will be used for job applications

---

## Known Open Threads

| Thread | Detail | Priority |
|---|---|---|
| Save Netflix files | `Ketan_resume_Netflix_AE.md` + `motivation_letter_netflix.md` — chat output only; parent dir exists | 🔴 High — do first next session |
| Save ABN AMRO files | Role 3 resume, Role 4 resume, motivation letter exist only as chat output | 🔴 High |
| `abn/` folder creation | Folder `personal/career/resumes/abn/` doesn't exist yet — run `mkdir -p` before any file writes | 🔴 Blocking ABN file saves |
| Submit Netflix application | Resume + motivation letter ready once saved to disk; not yet submitted | 🟡 Medium |
| LinkedIn handle verification | `linkedin.com/in/ketan-sahu` — confirm correct before submitting any application | 🟡 Medium — before submitting |
| Azure DevOps ATS gap (ABN Role 4) | JD lists Azure DevOps; user removed it from resume; potential ATS filter miss | 🟡 Medium — worth a single line in skills |
| Commit `copilot-instructions.md` | Language section added 2026-05-03; uncommitted | 🟡 Medium |
| ThoughtSpot in ABN Role 1 | Not in CDO JD; minor noise | 🟢 Low — cosmetic |
| ABN Role 2 resume | Never discussed; unclear if needed | 🟢 Low — confirm with Ketan |
| Commit ABN resume files | Role 1 modified but not committed | 🟡 Medium |

---

## ⚠️ Persistent File-Save Gotcha

**Pattern observed across two sessions (2026-05-01, 2026-05-03):** Files reported as created/saved actually do not exist on disk. The `create` tool silently fails if the parent directory doesn't exist, and chat output is not a substitute for on-disk files.

**Mandatory protocol for all file saves going forward:**
1. `bash: ls <parent-dir>` — confirm parent exists
2. `bash: mkdir -p <parent-dir>` — create if missing
3. `create` tool — write the file
4. `bash: ls <full-path>` — **verify the file is there before reporting ✅**

---

## Working Rules (from `.github/copilot-instructions.md`)

- **No PDF generation** unless explicitly requested
- **No table formatting in resumes** — use plain text, bold labels, or bullets only
- **Advisor behaviour:** challenge bad decisions, state trade-offs, hold positions under pressure
- Disagreement is not disrespect — best outcome > comfortable conversation
- **American English for all career documents** — organization, behavior, analyze, optimize, center (added 2026-05-03)

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
├── Ketan_resume_ABN.md                ← ABN Role 1 (CDO DE) — on disk ✅, not committed
├── Ketan_resume-AI-Augmented-DE.md    ← General AI-augmented DE resume — on disk ✅
├── Ketan_resume_Netflix_AE.md         ← Netflix Senior AE — ❌ NOT ON DISK (chat only)
├── motivation_letter_netflix.md       ← Netflix motivation letter — ❌ NOT ON DISK (chat only)
├── Letter of recommendation.md        ← Jeremy Boeijink / Odido — on disk ✅
└── abn/                               ← ⚠️ FOLDER DOES NOT EXIST YET
    ├── Ketan_resume_ABN_role3.md      ← ABN Role 3 (F&R Platform) — chat only ❌
    ├── Ketan_resume_ABN_role4.md      ← ABN Role 4 (Credit Risk Services) — chat only ❌
    └── motivation_letter_role4.md     ← ABN Role 4 motivation letter — chat only ❌
```
