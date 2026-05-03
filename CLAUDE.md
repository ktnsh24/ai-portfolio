# CLAUDE.md — AI Portfolio Session Audit Log

> Append-only. Each session is a new entry at the bottom.
> Last updated: 2026-05-03

---

## Session — 2026-05-01 — ABN AMRO Applications: Resume Suite + Motivation Letter (Role 4)

### What was done

- **Reviewed and edited Role 1 resume** (`personal/career/resumes/Ketan_resume_ABN.md`) — tailored for ABN AMRO CDO Data Engineer role; file modified on disk today
- **Drafted Role 3 resume** for ABN AMRO F&R Platform DE role — exists as chat output only, NOT yet saved to disk
- **Drafted Role 4 resume** for ABN AMRO Credit Risk Services Senior DE role — exists as chat output only, NOT yet saved to disk
- **Wrote motivation letter for Role 4** (Credit Risk Services Senior DE) — exists as chat output only, NOT yet saved to disk
  - Opening: "Dear Hiring Team"
  - 4 paragraphs: (1) why banking/AI angle, (2) current ML platform work at Odido, (3) Gen AI/Agentic AI hands-on from portfolio, (4) engineering craft + honest Azure framing
  - Ready to paste into portal — user must strip the markdown heading (lines 1–2, i.e. `# Motivation Letter…` and the blank line) before pasting

### ⚠️ Files that exist only as chat output (NOT saved to disk)

The session context referenced these paths, but none of them exist in the repo:

| Intended path | Status |
|---|---|
| `personal/career/resumes/abn/Ketan_resume_ABN.md` | ❌ `abn/` folder doesn't exist; Role 1 resume lives at `personal/career/resumes/Ketan_resume_ABN.md` |
| `personal/career/resumes/abn/Ketan_resume_ABN_role3.md` | ❌ Not saved — chat output only |
| `personal/career/resumes/abn/Ketan_resume_ABN_role4.md` | ❌ Not saved — chat output only |
| `personal/career/resumes/abn/motivation_letter_role4.md` | ❌ Not saved — chat output only |

**Next session must save these files to disk before continuing.**

### Decisions made

- Resume folder structure: use `personal/career/resumes/abn/` as the canonical subfolder for all ABN AMRO artefacts (Role 1 should eventually be moved there too for consistency)
- Motivation letter framing: lead with banking/data-governance angle (not generic ML), keep Azure honest (real Azure experience from AVEVA + Odido ADF patterns; no fabrication), signal Gen AI hands-on via ai-portfolio repos
- Azure DevOps in Role 4 resume: user **removed** Azure DevOps from the resume even though the JD lists it; decision was intentional but carries ATS risk (see open threads)
- No PDF generation unless explicitly requested (per `.github/copilot-instructions.md` rule)
- No table formatting in resumes (per `.github/copilot-instructions.md` rule)

### Gotchas discovered

- **`abn/` subfolder was never created** — referenced throughout the session but doesn't exist; any file-save instructions in chat pointed to a non-existent path
- **LinkedIn placeholder not confirmed** — all resumes use `linkedin.com/in/ketan-sahu`; Ketan needs to verify this is the correct handle before submitting
- **ThoughtSpot in Role 1 skills** — not in CDO JD; minor ATS noise; flag for cleanup
- **Copilot instructions (`copilot-instructions.md`) has uncommitted changes** — `git status` shows it as modified; should be committed

### Files changed

| Repo | File | What changed |
|------|------|--------------|
| ai-portfolio | `personal/career/resumes/Ketan_resume_ABN.md` | Edited (Role 1 CDO DE tailoring) — on disk, not yet committed |
| ai-portfolio | `.github/copilot-instructions.md` | Modified (uncommitted — content unknown, likely working-rules update) |
| ai-portfolio | `docs/shared/hands-on-labs/how-to-read-labs.md` | Modified (uncommitted — part of lab centralisation work, separate from career session) |

### Open threads / Next steps

1. **PRIORITY — Save unsaved files:** Open the Role 3, Role 4 resumes and motivation letter from chat history and save them under `personal/career/resumes/abn/`. Create the `abn/` folder first.
2. **Commit Role 1 resume** (`Ketan_resume_ABN.md`) — currently modified but not committed
3. **Confirm LinkedIn handle** — verify `linkedin.com/in/ketan-sahu` is correct; update all 3 resumes and letter if not
4. **Azure DevOps ATS gap (Role 4)** — JD lists Azure DevOps; resume omits it; consider adding a brief mention (e.g. "Azure DevOps (CI/CD pipelines)") in the skills section to close the gap
5. **ThoughtSpot cleanup (Role 1)** — not in CDO JD; remove or move to a less prominent position
6. **Commit `.github/copilot-instructions.md`** — has uncommitted changes
7. **Commit `docs/shared/hands-on-labs/how-to-read-labs.md`** — has uncommitted changes (lab centralisation work)
8. **Role 2 resume** — not discussed today; check if ABN AMRO Role 2 still needs a tailored resume

---

## Session — 2026-05-03 — Netflix Analytics Engineer Application (Resume + Motivation Letter)

### What was done

- **Netflix Senior Analytics Engineer resume drafted** — intended path `personal/career/resumes/Ketan_resume_Netflix_AE.md`
  - Tailored for Legal org / Content Enterprise DS&E team
  - Analytics-forward framing: KPI ownership, metric design, stakeholder translation, data storytelling
  - Claude Code named explicitly (matches JD requirement)
  - AI Portfolio section in bullet format (no tables)
  - No Tableau listed (honest gap — Power BI is primary; Streamlit noted in portfolio context)
  - Experience framed as "6+" (JD asks 7 — minor gap, not a blocker)
  - CET timezone noted naturally in summary

- **Netflix motivation letter drafted** — intended path `personal/career/resumes/motivation_letter_netflix.md`
  - 4 paragraphs: (1) why Netflix / AI workflow angle, (2) Odido domain ownership + anonymous stakeholder quote from recommendation letter, (3) AI portfolio specifics (RAG 13 eval labs, LangGraph, MCP, CrewAI), (4) CET + measurement integrity framing
  - American English throughout
  - Jeremy Boeijink's name removed — quote used anonymously ("one of my key business stakeholders")
  - Ready to paste into portal — strip header line if needed

- **American English rule added to `.github/copilot-instructions.md`** — `## Language` section added; confirmed present on disk and in `git status` as modified (uncommitted)

- **Recommendation letter reviewed** — `personal/career/Letter of recommendation.md`
  - Written by Jeremy Boeijink, Channel Manager, Commercial Management, Odido
  - Strong for this role: business stakeholder (not tech manager) validates analytical credibility and stakeholder partnership
  - Jeremy confirmed aware the letter will be used for job applications
  - Strategy: submit as additional document in Netflix portal; also useful at interview stage

### ⚠️ Files that exist only as chat output (NOT saved to disk)

Same silent-failure pattern as 2026-05-01 ABN AMRO session. Session summary reported ✅ but **`ls` confirmed files not present**.

| Intended path | Actual status |
|---|---|
| `personal/career/resumes/Ketan_resume_Netflix_AE.md` | ❌ Not on disk — chat output only |
| `personal/career/resumes/motivation_letter_netflix.md` | ❌ Not on disk — chat output only |
| `personal/career/resumes/abn/Ketan_resume_ABN_role3.md` | ❌ Still not on disk (carried over from 2026-05-01) |
| `personal/career/resumes/abn/Ketan_resume_ABN_role4.md` | ❌ Still not on disk (carried over from 2026-05-01) |
| `personal/career/resumes/abn/motivation_letter_role4.md` | ❌ Still not on disk (carried over from 2026-05-01) |

**Root cause:** `abn/` folder never created. Netflix files failed silently for same reason or tool did not write them. **Fix: always run `mkdir -p <folder>` via bash tool, then use `create` tool, then verify with `ls`.**

### Decisions made

- Jeremy's name removed from motivation letter — anonymous quote is stronger in applicant's own voice; name belongs in the recommendation letter only
- Recommendation letter strategy: submit as additional document in portal; resurface at interview stage
- American English is now a permanent rule in `copilot-instructions.md`
- No Tableau in Netflix resume — honest; Power BI is the parallel tool

### Gotchas discovered

- **Files reported ✅ in session summary but not on disk** — the `create` tool (or chat output) silently fails when the parent directory doesn't exist or the tool isn't invoked; always verify with `ls` after any file creation
- **`abn/` folder still does not exist** — every session that references it must run `mkdir -p` first before any file writes

### Files changed

| Repo | File | What changed |
|------|------|--------------|
| ai-portfolio | `.github/copilot-instructions.md` | Added `## Language` section (American English rule) — on disk ✅, uncommitted |
| ai-portfolio | `personal/career/resumes/Ketan_resume_Netflix_AE.md` | Intended creation — **NOT on disk** ❌ |
| ai-portfolio | `personal/career/resumes/motivation_letter_netflix.md` | Intended creation — **NOT on disk** ❌ |

### Unfinished / Next steps

1. **PRIORITY 1 — Save Netflix files to disk:**
   ```bash
   # Verify parent dir exists (it should):
   ls personal/career/resumes/
   # Then use create tool for Ketan_resume_Netflix_AE.md and motivation_letter_netflix.md
   # Then verify: ls personal/career/resumes/Ketan_resume_Netflix_AE.md
   ```
2. **PRIORITY 2 — Save ABN AMRO files to disk (carried over from 2026-05-01):**
   ```bash
   mkdir -p personal/career/resumes/abn/
   # Then create Role 3 resume, Role 4 resume, motivation letter from chat history
   # Then verify: ls personal/career/resumes/abn/
   ```
3. **Commit `copilot-instructions.md`** — Language section added, uncommitted
4. **Confirm LinkedIn handle** — `linkedin.com/in/ketan-sahu` still unverified; check before submitting Netflix application
5. **Netflix application — not yet submitted** — resume + motivation letter ready once saved to disk
6. **ABN AMRO Role 4 — Azure DevOps ATS gap** — JD lists it; resume omits it; accepted risk, worth one revisit before submitting

---
