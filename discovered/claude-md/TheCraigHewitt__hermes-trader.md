---
name: TheCraigHewitt__hermes-trader
source: https://github.com/TheCraigHewitt/hermes-trader/blob/9a5265ba9e2c4103b42fe57992f0db71215bf20e/claude.md
repo: TheCraigHewitt/hermes-trader
kind: claude-md
stars: 0
last_pushed: 2026-05-08T01:32:58Z
license: mit
score: 8
domains: [trading, agents-ai, safety-security]
tags: [guardrails, state-management, operational-integrity]
curated: 2026-06-14
curated_by: config-scout
---

# TheCraigHewitt/hermes-trader — claude-md

**Why it's worth keeping:** It treats the file system as a structured state machine via atomic helpers and prohibits manual tampering with historical records or strategy parameters to ensure traceability.

**Summary:** Enforces strict operational guardrails for an agentic trading system, focusing on memory integrity and preventing unauthorized rule changes during live windows.

**Source credibility:** Low-visibility repository, likely a niche or private trading project given 0 stars.

**Recency:** Current; uses modern Python tooling like uv.

**Source:** [TheCraigHewitt/hermes-trader/claude.md](https://github.com/TheCraigHewitt/hermes-trader/blob/9a5265ba9e2c4103b42fe57992f0db71215bf20e/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Editing Instructions

- Never edit `memory/` by hand mid-run. Runtime writes must go through atomic memory helpers.
- Never modify past journals, plans, or reflections. They are public commitments and receipts.
- Never relax guardrails: paper-only default, account isolation, position caps, drawdown halt, cost halt, universe lock.
- Never change `hermes.md`, `memory/strategy.md`, `agent/prompts/*.md`, or guardrail thresholds during the live held-out window except crash-only bug fixes documented in journals.
- Use Python 3.11+ and `uv`. No `requirements.txt`.
- Write tests before behavior changes.
```

</details>
