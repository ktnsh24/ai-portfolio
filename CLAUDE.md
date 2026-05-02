# CLAUDE.md — AI Portfolio Session Audit Log

> Append-only. Each session is a new entry at the bottom.
> Last updated: 2026-05-01

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
