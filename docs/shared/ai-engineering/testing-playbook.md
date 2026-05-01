# Testing Playbook (Shared)

> Cross-repo testing baseline for all ai-portfolio projects.

## What this standardizes

- Test pyramid structure (unit, integration, e2e)
- Deterministic test patterns (fixtures, stubs, seeded inputs)
- Quality gates (format, lint, tests)
- Reporting language (what to measure and how to summarize)

## Baseline test pyramid

| Layer | Purpose | Typical scope |
| --- | --- | --- |
| Unit | Validate isolated logic | Functions, model validation, adapters |
| Integration | Validate subsystem interactions | Route to service to storage/tool |
| End-to-end | Validate user-visible behavior | API contract + runtime wiring |

## Required quality gates

1. Format and lint must pass.
2. Unit tests must pass before integration tests.
3. Integration failures must include one reproducible command.
4. New features must include at least one happy-path and one error-path test.

## Reporting template

Use this table in repo docs when summarizing test quality:

| Metric | Value | Notes |
| --- | --- | --- |
| Unit tests | n | Core logic coverage |
| Integration tests | n | Route/service contracts |
| End-to-end checks | n | Runtime confidence |
| Known gaps | text | Risk accepted intentionally |

## DE parallel

This is the same discipline as pipeline validation: schema/unit checks first, integration checks next, then full pipeline smoke tests before release.
