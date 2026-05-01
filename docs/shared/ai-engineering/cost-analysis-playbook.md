# Cost Analysis Playbook (Shared)

> Cross-repo cost-analysis baseline for all ai-portfolio projects.

## What this standardizes

- Monthly cost framing (development vs small production)
- Service-by-service breakdown structure
- Cost guardrails and budget-protection section
- Trade-off analysis (cost vs latency vs quality)

## Required sections

1. Monthly cost summary
2. Service-by-service breakdown
3. Cost-saving levers
4. Alternative architecture cost comparison
5. Budget guard and operational limits

## Reporting template

Use this table shape for consistency across repos:

| Service | Dev estimate | Small prod estimate | Primary cost driver |
| --- | --- | --- | --- |
| LLM inference | value | value | Input/output token volume |
| Retrieval/storage | value | value | Query volume + index/storage |
| Runtime hosting | value | value | Request throughput + uptime |
| Observability | value | value | Log/metric volume |

## Cost guard baseline

- Set monthly budget limits per environment.
- Prefer local mode for iterative development.
- Keep provider-specific notes explicit (AWS, Azure, local).
- Document test-run cost separately from production operation cost.

## DE parallel

Treat model tokens like compute spend in batch jobs: optimize high-volume operators first, then optimize infra overhead.
