---
name: heyallencao__KeyStore__skill
source: https://github.com/heyallencao/KeyStore/blob/4547e74b382338985df4db5b4b5da650ea2d5caa/operation/ship/SKILL.md
repo: heyallencao/KeyStore
kind: skill
stars: 166
last_pushed: 2026-04-25T07:55:02Z
license: mit
score: 9
domains: [devops, cli-tools, software-engineering]
tags: [deployment, cicd, automation, reliability]
curated: 2026-06-15
curated_by: config-scout
---

# heyallencao/KeyStore — skill

**Why it's worth keeping:** The dual-mode ('advisory' vs 'project-adapted') logic provides a safety guardrail against destructive actions in unknown environments; the embedded shell scripts for dependency and migration auditing are highly portable and practical.

**Summary:** Automates the critical 'ship' phase by detecting CI/CD environments and executing a multi-step verification, test, and deployment pipeline.

**Source credibility:** High-quality personal framework with significant community interest (166 stars) and recent maintenance.

**Recency:** Current; perfectly suited for modern agentic workflows using tool-calling and terminal execution.

**Source:** [heyallencao/KeyStore/operation/ship/SKILL.md](https://github.com/heyallencao/KeyStore/blob/4547e74b382338985df4db5b4b5da650ea2d5caa/operation/ship/SKILL.md) · 166★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ks-ship
description: "Delivery closeout before release. Accepts review-approved changes, runs the final checks, generates execution guidance, and performs merge/deploy/canary only when the project is explicitly adapted for it."
layer: operation
owner: ship
inputs:
  - review_report
  - qa_report
outputs:
  - deployment_result
  - ship_result
entry_modes:
  - build-ready
  - release-ready
---

> Preamble: see [templates/preamble.md](../../templates/preamble.md)

# Ship

Delivery closeout between review/QA and release. Detects CI/CD config, runs final checks, and executes or advises merge/deploy/canary. Only executes when the project provides the required commands; otherwise stays advisory.

**Enter when**: review passed and (`qa_required = false` or `qa_result = pass|partial`). Do not enter when QA is still running or a severe problem needs diagnosis. **Not responsible for**: code review, QA execution, the final release decision.

## Compliance Anchors

> **Never guess the target branch or deploy command.**
>
> **In advisory mode, do not write `ship_result = done`.**
>
> **If QA was skipped or partial, that fact must appear in the ship report.**

## Modes

| Mode | When |
```

</details>
