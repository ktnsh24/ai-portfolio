# How to Read Hands-On Labs (Shared Guide)

> Central, repo-agnostic guidance for all ai-portfolio labs.

## Table of Contents

- [Who this is for](#who-this-is-for)
- [Mode policy (required)](#mode-policy-required)
- [The core lab pattern](#the-core-lab-pattern)
- [Default learner order](#default-learner-order)
- [How comparison works in one result panel](#how-comparison-works-in-one-result-panel)
- [Repo index](#repo-index)
- [When a lab must be mode-specific](#when-a-lab-must-be-mode-specific)

## Who this is for

Use this guide before running labs in any repo under ai-portfolio. It defines one consistent way to write, run, and interpret labs so newcomers do not need to relearn the format in every repo.

## Mode policy (required)

- Default writing style in lab docs is generic and mode-agnostic.
- A lab is mode-specific only when the doc explicitly declares a Mode flag.
- Preferred default mode for comparative evaluation labs is combined.
- Alternative modes stay documented as comments/examples, not as the default path.

Recommended `.env` snippet:

```dotenv
# Preferred for labs: show both lanes side by side
EVAL_MODE=combined

# Alternatives (use only when needed)
# EVAL_MODE=rule_based
# EVAL_MODE=llm_judge
```

## The core lab pattern

For every lab, keep the same structure:

1. One knob changes.
2. One hypothesis is stated.
3. Same baseline questions are used.
4. Same score columns are reported.
5. One operational takeaway is written.

This is the same engineering loop as A/B testing in pipelines: change one transform, keep the test dataset fixed, compare metrics, keep or revert.

## Default learner order

For first-time readers, keep the progression linear:

1. Lab 1: baseline setup and first measurement
2. Lab 2: first quality/safety control
3. Lab 3: first business or operational signal
4. Lab 4: first production-hardening control

After 1-4 are understood, continue with advanced labs (retrieval tuning, monitoring, judge policy, protocol tuning, or agent orchestration depending on repo).

## How comparison works in one result panel

When combined mode is used, both lanes appear together in one panel/table for the same question:

| Field | Meaning |
| --- | --- |
| `rule_based.overall_score` | Deterministic heuristic score |
| `llm_judge.overall_score` | Judge-model semantic score |
| `score_delta` | `llm_judge - rule_based` |
| `agreement_band` | agrees / partial / diverges |
| `policy_hint` | keep, review, or escalate |

This keeps comparison immediate and removes context-switching between different output locations.

## Repo index

| Repo | GitHub | Local docs root | Primary lab set |
| --- | --- | --- | --- |
| rag-chatbot | [ktnsh24/rag-chatbot](https://github.com/ktnsh24/rag-chatbot) | [repos/rag-chatbot/docs](../../../repos/rag-chatbot/docs) | RAG + eval + judge |
| ai-gateway | [ktnsh24/ai-gateway](https://github.com/ktnsh24/ai-gateway) | [repos/ai-gateway/docs](../../../repos/ai-gateway/docs) | gateway + routing + cache |
| ai-agent | [ktnsh24/ai-agent](https://github.com/ktnsh24/ai-agent) | [repos/ai-agent/docs](../../../repos/ai-agent/docs) | tool-using agent |
| mcp-server | [ktnsh24/mcp-server](https://github.com/ktnsh24/mcp-server) | [repos/mcp-server/docs](../../../repos/mcp-server/docs) | protocol tuning |
| ai-multi-agent | [ktnsh24/ai-multi-agent](https://github.com/ktnsh24/ai-multi-agent) | [repos/ai-multi-agent/docs](../../../repos/ai-multi-agent/docs) | orchestration |
| knowledge-engine | [ktnsh24/knowledge-engine](https://github.com/ktnsh24/knowledge-engine) | [repos/knowledge-engine/docs](../../../repos/knowledge-engine/docs) | GraphRAG + KB |

## When a lab must be mode-specific

Mark a lab as mode-specific only if one of these is true:

- It validates judge-vs-rule disagreement behavior.
- It validates provider-specific protocol behavior.
- It validates transport semantics that do not exist in other modes.

Suggested label format in docs:

```markdown
**Mode:** generic
```

or

```markdown
**Mode:** specific (`combined` required)
```
