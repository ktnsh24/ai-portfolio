# CLAUDE.md — AI Portfolio Session Audit Log

> Append-only. Each session is a new entry at the bottom.
> Last updated: 2026-05-13

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

## Session — 2026-05-04 — I5: Wire /v1/get_bna to ProcessInteractor (ITMM-55945)

### What was done

- **I4 confirmed merged** — PR #83 is the I4 CallCentre Integrator merge; `main` now includes I4. Branch `feature/itmm-55945` cuts from that merge commit.
- **I5 implementation complete** — All files written, 12 new tests passing (392 total, 2 pre-existing failures unrelated to I5), NOT yet committed. Local curl testing in progress at session end.
- **WAF/TYK 403 resolved** — RC's connectivity issue was a wrong API key (not WAF). Key is stored in AWS Secrets Manager — do not hardcode here. RC IPs `3.125.232.134` and `3.121.145.138` already whitelisted in `aws_wafv2_ip_set.salesforce`.
- **BlueConic new endpoint scoping** — Teams message template written with 7 questions for BlueConic team (request payload, response shape, HTTP method, volume, auth, error handling, environments). Not yet sent.
- **Debug log line added to v1.py (line 48)** — `logger.info("DEBUG use_process_interactor=%s", settings.use_process_interactor)` — temporary, added to confirm flag value at runtime. **MUST BE REMOVED before committing.**

### Decisions made

- `process_interactor_source` tracking field added to `BnaEventContext` TypedDict (no default — TypedDict all-keys required) and `BnaEvent` Pydantic model (default `None`). Values: `"process_interactor"` | `"fallback"` | `None`.
- Old callers of `record_bna_event` / `set_event_in_state` unaffected — new params default to `None`.
- Fallback is **silent to the customer** — Sentry notified, old `process_request()` path takes over transparently.
- `to_bna_response()` in `adapters.py` applies identical action_label lookup as old path: B2C direct, B2B via `map_to_internal_action_id`.
- `ProcessInteractorError` raised by adapter when EventProcessor returns non-200 — caught in route layer to trigger fallback.
- `mock_orchestrator_settings` fixture required in tests 1, 3, 4, 5 because old path always calls `get_orchestrator_settings()` at line 112 of v1.py.

### Gotchas discovered

- **Pre-existing test failures** — `test_should_report_502_on_upstream_name_error` fails on `main` before I5 changes. Confirmed NOT caused by I5. Do not fix as part of this story.
- **TypedDict has no defaults** — `BnaEventContext` is a TypedDict, so new fields must be truly optional (use `total=False` or `NotRequired`) or all callers must pass them. Existing callers pass `process_interactor_source=None` — works because new params have defaults in function signatures.
- **AWS keys expire** — dev account 770939618751 keys loaded via `export $(grep -E "^AWS_" .env | xargs)`. If expired, refresh from https://tmnl.awsapps.com/start
- **Server process not killed between restarts** — old PID (82773) kept serving with stale `.pyc` cache even after apparent restart. Must explicitly `kill $(pgrep -f "api_proxy.main")` before restarting. This was the cause of new PI path not being confirmed at session end.
- **Test customer identity table mismatch** — `tmnl-bna-dev-customer-settings` has 1274 customers but NOT all exist in `tmnl-bna-dev-shared-infra-customer-identity`. The identity table determines `business_unit`. Must use a customer present in BOTH tables.
  - ✅ **Good test customer (B2C):** `gWtqTM2LWgzJ8mJrPI4mXMOiDD9jzUFL4t+ahqgdbek=` — in identity table
  - ❌ **Bad test customer:** `ZiTMlUCEt8TOlLeba12ebThryM1l0cFFIjq5oUPgTKA=` — in customer-settings only, NOT in identity table

### Files changed

| Repo | File | What changed |
|------|------|-------------|
| maestro-devops-shared-proxy | `api_proxy/api_proxy/process_interactor/adapters.py` | NEW — `ProcessInteractorError`, `to_bna_response()` |
| maestro-devops-shared-proxy | `api_proxy/api_proxy/event_logging/models.py` | Added `process_interactor_source` to `BnaEventContext` + `BnaEvent` |
| maestro-devops-shared-proxy | `api_proxy/api_proxy/domain/logging.py` | Added `process_interactor_source` param to `set_event_in_state()` + `record_bna_event()` |
| maestro-devops-shared-proxy | `api_proxy/api_proxy/api/v1.py` | Added `use_process_interactor` branch to `get_bna` route, module-level logger, Settings dep — **⚠️ has temp debug line at line 48 to remove** |
| maestro-devops-shared-proxy | `api_proxy/tests/api/test_v1_get_bna_pi.py` | NEW — 6 tests (flag off, happy path, exception fallback, non-200 fallback, response contract, source field) |
| maestro-devops-shared-proxy | `api_proxy/tests/process_interactor/test_adapters.py` | NEW — 6 tests (B2C label, B2B label, missing label, 400 raises, 500 raises, missing statusCode raises) |

### Unfinished / Next steps

1. **IMMEDIATE — Remove debug log line from v1.py (line 48):** `logger.info("DEBUG use_process_interactor=%s", ...)` before committing.
2. **IMMEDIATE — Restart server properly** to confirm new PI path fires:
   ```bash
   kill $(pgrep -f "api_proxy.main")
   cd /home/ketan-odido/maestro/maestro-devops-shared-proxy/api_proxy
   export $(grep -v "^#" .env | xargs)
   .venv/bin/python -m api_proxy.main
   ```
   Then curl with good test customer `gWtqTM2LWgzJ8mJrPI4mXMOiDD9jzUFL4t+ahqgdbek=` and confirm `DEBUG use_process_interactor=True` in logs.
3. **Commit I5** — `feat(process-interactor): wire /v1/get_bna to EventProcessor with fallback (ITMM-55945)`. Run pre-commit checklist + Claude Opus cross-model review before pushing.
4. **Push + open PR** for `feature/itmm-55945`.
5. **I6** — Wire `/v1/post_event` + `predict_for_channel()` to EventProcessor (same try/fallback pattern).
6. **I7** — Wire `/v3/blueconic/event` with `asyncio.gather` parallel + mixed fallback.
7. **I8** — Integration tests + Sentry alert + latency comparison + validation runbook.
8. **I9** — Remove `process_event` sidecar (7-day gate after I8 confirmed clean).

---

## Session — 2026-05-05 — I5: Local Testing Complete + Pre-existing Bug Fix (ITMM-55945)

### What was done

- **I5 end-to-end local test confirmed working** — Swagger request via `POST /v1/get_bna` with real B2C customer returned `next_best_action_id: "1"` (`"Bied Thuis aan"`) via the process interactor path. Log line `"get_bna handled by process_interactor"` confirmed in terminal. Total latency 941ms.
- **Full test suite run** — 113 passed, 1 failed (pre-existing). All 12 new I5 tests pass.
- **Pre-existing bug fixed** — `test_should_report_502_on_upstream_name_error` was failing with 504 instead of 502. Root cause: (1) `backoff` in `request.py` was retrying on `ConnectError` (DNS failures) — after 3 retries it timed out with `ConnectTimeout` which hit the 504 branch instead of 502; (2) the test itself had no mock, making a real network call. Both fixed — test now passes (0 failures, 115 passed).
- **Test evidence document created** — written in plain language, no abbreviations, covers the full request flow from Swagger through all DynamoDB lookups to the model and back. Placed in charm repo.
- **CLAUDE.md misplaced file deleted** — `/home/ketan-odido/maestro/maestro-devops-shared-proxy/CLAUDE.md` (untracked) deleted in a prior session.

### Decisions made

- Pre-existing `test_should_report_502_on_upstream_name_error` bug was fixed proactively — not related to I5 but fixed to avoid carrying technical debt forward.
- `giveup=lambda e: isinstance(e, httpx.ConnectError)` added to backoff — DNS failures are permanent errors, not worth retrying.
- Test now mocks `Resources.internal_httpx_json_client` to raise `ConnectError` deterministically — no more real network call in this test.
- Test evidence document placed in `maestro-devops-shared-proxy-charm` repo (not shared-proxy) under `api_proxy/docs/process_interactor/`.

### Gotchas discovered

- **`no_action_available` root cause** — if `action_channel_inclusion_flags` is empty/missing in DynamoDB `tmnl-bna-dev-customer-settings`, the eligibility matrix is all-zeros and the model returns `no_action_available`. Always use a customer with flags set for the requested channel.
- **Line 3 warning (`empty bna_event_context`) is expected** — the response middleware runs before the `record_bna_event` background task. Middleware sees empty context and skips its Kinesis write. Background task still fires. This is a known gap — Kinesis alignment is out of I5 scope.
- **Salesforce response shape** — only `next_best_action_id` and `action_label` are consumed by Salesforce. Other fields (`prediction_id`, `request_id`, `bna_ids_per_channel`, `ai_banner_message`, etc.) exist in the model but are `null` for standard call centre requests.

### Files changed

| Repo | File | What changed |
|------|------|-------------|
| maestro-devops-shared-proxy | `api_proxy/api_proxy/domain/request.py` | Added `giveup=lambda e: isinstance(e, httpx.ConnectError)` to backoff decorator — fixes 504→502 on DNS failures |
| maestro-devops-shared-proxy | `api_proxy/tests/api/test_v1.py` | Added `Resources` import + explicit `ConnectError` mock to `test_should_report_502_on_upstream_name_error` |
| maestro-devops-shared-proxy-charm | `api_proxy/docs/process_interactor/i5-local-test-evidence.md` | NEW — full local test evidence document |

**Still uncommitted (carried over from 2026-05-04 session):**
- `api_proxy/api_proxy/api/v1.py` — I5 process interactor branch
- `api_proxy/api_proxy/domain/logging.py` — `process_interactor_source` param
- `api_proxy/api_proxy/event_logging/models.py` — `process_interactor_source` field
- `api_proxy/api_proxy/process_interactor/event_processor.py` — datetime fix
- `api_proxy/api_proxy/process_interactor/adapters.py` — NEW
- `api_proxy/tests/api/test_v1_get_bna_pi.py` — NEW (6 tests)
- `api_proxy/tests/process_interactor/test_adapters.py` — NEW (6 tests)

### Open threads / Next steps

1. **PRIORITY — Commit I5** on `feature/itmm-55945`:
   ```
   feat(process-interactor): wire /v1/get_bna to EventProcessor with fallback (ITMM-55945)
   
   Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>
   ```
2. **Push + open PR** for `feature/itmm-55945` — ready to go, 0 test failures.
3. **I6** — Wire `/v1/post_event` + `predict_for_channel()` to EventProcessor using same try/fallback pattern.
4. **I7** — Wire `/v3/blueconic/event` with `asyncio.gather` parallel + mixed fallback.
5. **I8** — Integration tests + Sentry alert + latency comparison + validation runbook.
6. **I9** — Remove `process_event` sidecar (7-day gate after I8 confirmed clean).
7. **Kinesis alignment** — the `empty bna_event_context` warning on process interactor requests needs proper alignment with Kinesis event logging (future story, not I5).

---

## Session — 2026-05-06 — I5: Review #2 Fixes Complete + Full Suite Green (ITMM-55945)

### What was done

- **Completed all Opus review #2 fixes** — all outstanding items from the code review are resolved:
  - BLOCKER: `v1.py` exception narrowing, `logger.bind(pi_source=...)`, fallback log → error, `next_prediction_id` + `next_ai_banner_message` added to `record_bna_event` call (already done in prior session, verified)
  - HIGH: `adapters.py` raises `ProcessInteractorError` on missing `statusCode` or `body` keys (already done, verified)
  - Test #6 (`test_get_bna_pi_source_set_in_event_context`): uses `write_event.assert_awaited_once()` + hard field assertion — **passes**
  - LOW: `process_interactor_source` comment mirrored on TypedDict field in `event_logging/models.py` line 37 — already present, verified
  - MEDIUM: `get_orchestrator_settings` confirmed `@cache` decorated in `domain/dynamodb.py`

- **Fixed test suite hangs caused by local env** — `USE_PROCESS_INTERACTOR=true` in local `.env` caused pre-existing tests that hit `/v1/get_bna` without a settings override to hang on DynamoDB calls. Fixed by adding `autouse=True` fixture `reset_settings_override` in `tests/api/conftest.py` that defaults `use_process_interactor=False` for all tests and cleans up `dependency_overrides[get_settings]` after each test. I5 tests override the setting explicitly in their test body.

- **Full test suite: 381 passed, 2 failed (pre-existing)** — the 2 failures (`test_feature_flag_default_disabled`, `test_use_process_interactor_defaults_to_false`) exist on `main` before I5 changes; caused by `USE_PROCESS_INTERACTOR=true` in local `.env`, not by I5.

- **All changes staged, NOT yet committed** — user deferred commit to next session.

### Decisions made

- `autouse` fixture in conftest is the cleanest isolation: it centralises the default without touching every existing test individually. I5-specific tests override it with `_override_settings(use_process_interactor=True)` inside the test body.
- Removed the manual `app.dependency_overrides[get_settings] = ...` from `test_should_report_502_on_upstream_name_error` since autouse covers it.
- `Settings, get_settings` import removed from `test_v1.py` (no longer needed there).

### Gotchas discovered

- **autouse fixture ordering matters** — `reset_settings_override` runs first (sets flag OFF); I5 tests then call `_override_settings(use_process_interactor=True)` inside the test body which takes effect for that test only. After the test the autouse teardown (`yield` → `pop`) cleans the override. No state leaks.
- **Pre-existing 2 failures are env-only** — they call `get_settings()` directly (reads `.env`); no way to fix without either clearing `.env` or mocking `get_settings` in those tests. Out of I5 scope; will be moot in CI where `USE_PROCESS_INTERACTOR` defaults to `false`.

### Files staged (NOT yet committed) on `feature/itmm-55945`

| File | What changed |
|------|-------------|
| `api_proxy/api_proxy/api/v1.py` | I5 process interactor branch, BLOCKER fixes |
| `api_proxy/api_proxy/domain/logging.py` | `process_interactor_source` param |
| `api_proxy/api_proxy/domain/models.py` | (minor — check on commit) |
| `api_proxy/api_proxy/domain/request.py` | `giveup=ConnectError` backoff fix |
| `api_proxy/api_proxy/event_logging/models.py` | `process_interactor_source` field on TypedDict + BnaEvent |
| `api_proxy/api_proxy/process_interactor/adapters.py` | NEW — `to_bna_response()`, `ProcessInteractorError` |
| `api_proxy/api_proxy/process_interactor/event_processor.py` | datetime fix |
| `api_proxy/api_worker/events_worker.py` | (minor — check on commit) |
| `api_proxy/tests/api/conftest.py` | `reset_settings_override` autouse fixture + `Settings`/`get_settings` import |
| `api_proxy/tests/api/test_v1.py` | Removed manual settings override from 502 test; removed `Settings`/`get_settings` import |
| `api_proxy/tests/api/test_v1_get_bna_pi.py` | NEW — 6 I5 tests |
| `api_proxy/tests/process_interactor/test_adapters.py` | NEW — 7 adapter tests |
| `api_proxy/tests/process_interactor/test_event_processor.py` | Updated |

### Commit message to use tomorrow

```
feat(process-interactor): wire /v1/get_bna to EventProcessor with fallback (ITMM-55945)

- Add USE_PROCESS_INTERACTOR flag to route /v1/get_bna through local EventProcessor
- Transparent fallback to old process_request() path on any exception (Sentry notified)
- Add ProcessInteractorError: raised when EventProcessor returns non-200 status
- Add to_bna_response() adapter: maps EventProcessor dict → BnaResponseModel with B2C/B2B
  action label lookup matching the old path's semantics
- Add process_interactor_source field to BnaEventContext and BnaEvent for Athena observability
- Add backoff giveup on ConnectError to prevent retry loops on DNS failures
- Fix test suite env isolation: autouse fixture defaults use_process_interactor=False
- 381 tests passing (2 pre-existing env-only failures unrelated to I5)

Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>
```

### Open threads / Next steps

1. **PRIORITY — Commit I5** using commit message above, then push `feature/itmm-55945` and open PR
2. **I6** — Wire `/v1/post_event` + `predict_for_channel()` to EventProcessor (same try/fallback pattern)
3. **I7** — Wire `/v3/blueconic/event` with `asyncio.gather` parallel + mixed fallback
4. **I8** — Integration tests + Sentry alert + latency comparison + Athena DDL for `process_interactor_source` column + validation runbook
5. **I9** — Remove `process_event` sidecar (7-day gate after I8 confirmed clean) + narrow `except Exception` to `ProcessInteractorError`
6. **Kinesis alignment** — `empty bna_event_context` warning on process interactor path needs fixing (future story)

---

## Session — 2026-05-11 — I5 live in dev, PI flag deployed via feature branch

### What was done

- **PR #84 (I5) confirmed merged to `main`** (merged 2026-05-11T07:25:50Z) — `/v1/get_bna` wired to EventProcessor with fallback
- **Addressed final GitHub Copilot review round 2 (3 items) + fixed CI lint failure:**
  - `get_orchestrator_settings` keyword arg consistency (`@cache` key fix)
  - `NotRequired[str | None]` for `process_interactor_source` in `BnaEventContext` TypedDict
  - `AsyncMock` for `internal_httpx_json_client` patch in `test_v1.py`
  - Ruff formatter failure: long `patch.object` line split across 5 lines — commit `fa40209`
- **PR #85 opened** — `feature/enable-pi-flag-dev` — flips `USE_PROCESS_INTERACTOR` from `"false"` to `"true"` in `terraform/base/proxy_deployment.tf`
- **Feature branch deploy workflow ran automatically** on push to `feature/enable-pi-flag-dev` — Terraform applied to dev, flag is `true` in ECS task (confirmed via ECS console)
- **Local PI path confirmed working** — `get_bna handled by process_interactor` log line visible in local terminal when running against localhost:8000/5003
- **Dev ECS CloudWatch verification pending** — API Gateway URL + API key needed; local testing confirmed code correct but dev endpoint not yet hit via Postman/curl
- **API key removed from CLAUDE.md** — was accidentally committed in 2026-05-04 session; removed and replaced with "stored in AWS Secrets Manager"

### Decisions made

- Feature branch deploy workflow (`deploy-dev-feature.yml`) triggers automatically on `feature/**` push — no need to modify deploy.yml or wait for PR merge to test in dev
- Swagger UI (`/docs`) is NOT exposed via API Gateway (VPC-linked, internal) — use Postman + `x-api-key` header to hit dev endpoint
- Athena column for `process_interactor_source` requires `ALTER TABLE` by infra team (not Ketan's access) — deferred to I8
- PR #85 still needs merge so `main` doesn't revert the flag on next deploy from main

### Gotchas discovered

- **CloudWatch log group is NOT `/tmnl-bna-dev/tmnl-bna-dev-shared-infra`** — app logs go through Firelens/FluentBit; check `tmnl-bna-dev-shared-infra-firelens` log group instead
- **Feature branch Terraform deploy applies immediately** — no PR merge needed; flag was already live in dev 1 hour before this was discovered
- **`/docs` Swagger returns "Missing Authentication Token"** — API Gateway doesn't proxy `/docs` path; use Postman with `x-api-key` header
- **Dev API Gateway URL** — format: `https://<api-id>.execute-api.eu-central-1.amazonaws.com/tmnl-bna-dev-shared-infra/v1/get_bna`; API ID visible in AWS Console → API Gateway
- **AWS keys expire during day** — refresh from https://tmnl.awsapps.com/start when `UnrecognizedClientException` appears

### Files changed

| Repo | File | What changed |
|------|------|-------------|
| maestro-devops-shared-proxy | `api_proxy/tests/api/test_v1.py` | Ruff format fix — broke long `patch.object` line (commit `fa40209`) |
| maestro-devops-shared-proxy | `terraform/base/proxy_deployment.tf` | `USE_PROCESS_INTERACTOR` `"false"` → `"true"` (PR #85, feature branch deployed) |
| ai-portfolio | `CLAUDE.md` | Removed hardcoded API key from 2026-05-04 session |

### Unfinished / Next steps

1. **Get dev API Gateway URL + API key** — ask teammate; format: AWS Console → API Gateway → `tmnl-bna-dev-shared-infra` → Stages → copy Invoke URL
2. **Send Postman request to dev endpoint** — use customer `gWtqTM2LWgzJ8mJrPI4mXMOiDD9jzUFL4t+ahqgdbek=`; check `tmnl-bna-dev-shared-infra-firelens` log group for `get_bna handled by process_interactor`
3. **Merge PR #85** — so `main` stays in sync and flag doesn't revert on next deploy from main
4. **Monitor dev for 1 day** — no Sentry alerts = stable; then discuss prod rollout with team
5. **I6** — Wire `/v1/post_event` + `predict_for_channel()` to EventProcessor (same try/fallback pattern)
6. **I7** — Wire `/v3/blueconic/event` with `asyncio.gather` parallel + mixed fallback
7. **I8** — Athena DDL for `process_interactor_source` (needs infra team access), Sentry alert, latency comparison
8. **I9** — Remove `process_event` sidecar (7-day gate after I8 confirmed clean)


---

## Session — 2026-05-13 — Prod Incident: datetime bug fix + hotfix deployed

### What was done

- **Prod incident triggered** — PR #85 (flag flip to `true`) merged at ~12:50 UTC → `Deploy All Envs` auto-triggered → `USE_PROCESS_INTERACTOR=true` deployed to prod. First real prod traffic at 12:57 UTC hit the PI path and crashed.
- **3 Sentry alerts fired (SHARED-PROXY-8P, 8N, 8M):**
  - 8P: `TypeError: can't subtract offset-naive and offset-aware datetimes` in `base.py:calculate_latest_online_weights` — DynamoDB returns timezone-naive `creation_timestamp`; code subtracts from `datetime.now(timezone.utc)` which is aware
  - 8N: `ProcessInteractorError` in `adapters.py:to_bna_response` — caused by 8P cascade
  - 8M: `get_bna process_interactor fallback triggered` — fallback fired correctly, customers unaffected
  - 8Q: `RemoteProtocolError: Server disconnected` in `base.py:_send_req` — separate connection issue, already caught by `httpx.RequestError`
- **Hotfix PR #86 created and merged** — `hotfix/disable-pi-flag-prod` branch: flag back to `"false"` + urllib3 2.6.3→2.7.0 (2 high CVEs). Prod deploy blocked for hours by flaky `Integration Test Dev` ("Cannot find matching workflow run!" race condition).
- **Root cause identified** — Dev test customer `gWtqTM2LWgzJ8mJrPI4mXMOiDD9jzUFL4t+ahqgdbek=` had NO `creation_timestamp` in `customer_state` DynamoDB → fallback to `current_time` (same tz as `now(utc)`) → no crash. Prod customers have real historical timestamps stored WITHOUT tzinfo.
- **Fix implemented on `feature/datetime-fix`** — `base.py:calculate_latest_online_weights`: check `raw_ts.tzinfo is None` → `replace(tzinfo=timezone.utc)` before subtraction.
- **10 new tests added to `test_base_integrator.py`:**
  - `TestOnlineWeights` (7 new): naive timestamp doesn't raise, naive treated as UTC (decay applies), aware unchanged, missing timestamp, zero diff, multiple actions, missing action defaults 1.0
  - `TestSendEventProcessorConnectionErrors` (3 new): `RemoteProtocolError` retries, all retries exhausted raises, mixed errors then success
- **391 tests pass** (2 pre-existing env-only failures, not caused by fix)
- **Deployed to dev** via `feature/**` auto-deploy with `USE_PROCESS_INTERACTOR=true` temporarily in Terraform — dev is running fix+flag for Postman verification
- **Postman testing guide written** — 5 request scenarios covering predict/offer/reject + multiple channels

### Decisions made

- Fix normalises naive timestamps to UTC (treat as UTC — consistent with how prod data was always intended). Alternative (reject and log) was rejected — would still cause fallback on every prod customer.
- `feature/datetime-fix` branch includes temp flag `true` for dev testing only — Terraform flag must be reverted to `false` before opening the final PR to main.
- `RemoteProtocolError` is already a subclass of `httpx.RequestError` — no code change needed, just tests to confirm retry fires.
- Scenario 5 (unknown customer → 400) is pre-existing behaviour, not related to the fix. Removed from test matrix.

### Gotchas discovered

- **`Deploy All Envs` fires on EVERY merge to `main`** — including hotfix/flag-flip PRs. There is NO way to merge to main without triggering a prod deploy. Always consider prod impact before merging.
- **Dev test with current customer hid the bug** — customer had no stored `creation_timestamp` so code defaulted to `current_time` (timezone-aware) → no crash. Production customers have years of stored history. **Rule: when testing PI path in dev, always find a customer that has a `creation_timestamp` in `tmnl-bna-dev-customer-state` DynamoDB.**
- **Flaky `Integration Test Dev`** — "Cannot find matching workflow run!" is a race condition in the trigger script. Pre-existing issue tracked in draft PR #72. Workaround: re-run repeatedly OR get repo admin to bypass the gate.
- **`deploy-dev-feature.yml` only triggers on `feature/**` branches** — `fix/**` or `hotfix/**` branches do NOT trigger auto-deploy. Must rename to `feature/...` to use the shortcut.
- **Terraform state lock** — pushing twice to same feature branch in quick succession triggers two concurrent deploy workflows → second one fails with state lock. Safe to ignore if first run succeeded.
- **App logs NOT in CloudWatch** — go through FluentBit/Firelens → Elastic. CloudWatch `-firelens` log group only has FluentBit operational logs.

### Files changed

| Repo | File | What changed |
|------|------|-------------|
| maestro-devops-shared-proxy | `terraform/base/proxy_deployment.tf` | PR #85: `false`→`true` (caused incident); PR #86: `true`→`false` (hotfix); `feature/datetime-fix`: `false`→`true` (temp, dev-only) |
| maestro-devops-shared-proxy | `api_proxy/poetry.lock` | urllib3 2.6.3 → 2.7.0 (GHSA-mf9v-mfxr-j63j, GHSA-qccp-gfcp-xxvc) |
| maestro-devops-shared-proxy | `api_proxy/api_proxy/process_interactor/integrators/base.py` | Normalise timezone-naive `creation_timestamp` to UTC before subtraction |
| maestro-devops-shared-proxy | `api_proxy/tests/process_interactor/test_base_integrator.py` | +10 tests: 7 datetime variants + 3 RemoteProtocolError retry tests |

### Unfinished / Next steps

1. **PRIORITY — Verify fix in dev via Postman** — 5 scenarios listed above; check Elastic for `get_bna handled by process_interactor` WITHOUT fallback line. Need API Gateway URL + API key from teammate.
2. **After dev confirmed clean** — revert `terraform/base/proxy_deployment.tf` flag back to `"false"` on `feature/datetime-fix`, then open PR to main (code fix only, no flag).
3. **After fix PR merged to main** — separate small PR to flip flag `true` in prod via `feature/**` branch (same pattern as PR #85 but won't hit the datetime crash this time).
4. **Investigate flaky `Integration Test Dev`** — draft PR #72 exists; blocked deploy for hours today.
5. **Fix the "find a prod-like customer for dev testing" gap** — after fix is deployed, scan `tmnl-bna-dev-customer-state` to identify a customer with a real `creation_timestamp` for future regression testing.
6. **I6** — Wire `/v1/post_event` + `predict_for_channel()` to EventProcessor (same try/fallback pattern) — do NOT start until fix is confirmed in prod.
