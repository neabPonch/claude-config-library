---
name: LukasNiessen__terrashark
source: https://github.com/LukasNiessen/terrashark/blob/36bf2971c92f014b7eda67e4b2c8ccd9c9b37c05/SKILL.md
repo: LukasNiessen/terrashark
kind: skill
stars: 293
last_pushed: 2026-05-24T09:01:45Z
license: mit
score: 9
domains: [infrastructure-as-code, devops, security]
tags: [terraform, iac, risk-mitigation, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# LukasNiessen/terrashark — skill

**Why it's worth keeping:** It uses advanced 'Conditional Reference' loading logic to manage context window efficiency and implements a risk-first mental model through explicit failure mode diagnosis.

**Summary:** A specialized IaC orchestration workflow that focuses on diagnosing failure modes like identity churn and secret exposure rather than just generating HCL.

**Source credibility:** Strong; 293 stars indicates significant community traction and recent maintenance.

**Recency:** Very current; designed specifically for modern agentic workflows like Claude Code.

**Source:** [LukasNiessen/terrashark/SKILL.md](https://github.com/LukasNiessen/terrashark/blob/36bf2971c92f014b7eda67e4b2c8ccd9c9b37c05/SKILL.md) · 293★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: terrashark
description: "Prevent Terraform/OpenTofu hallucinations by diagnosing and fixing failure modes: identity churn, secret exposure, blast-radius mistakes, CI drift, and compliance gate gaps. Use when generating, reviewing, refactoring, or migrating IaC and when building delivery/testing pipelines."
---

# Terrashark: Failure-Mode Workflow for Terraform/OpenTofu

Run this workflow top to bottom.

## 1) Capture execution context

Record before writing code:
- runtime (`terraform` or `tofu`) and exact version
- provider(s), target platform, and state backend
- execution path (local CLI, CI, HCP Terraform/TFE, Atlantis)
- environment criticality (dev/shared/prod)

If unknown, state assumptions explicitly.

## 2) Diagnose likely failure mode(s)

Select one or more based on user intent and risk:
- identity churn: resource addressing instability, refactor breakage
- secret exposure: secrets in state, logs, defaults, artifacts
- blast radius: oversized stacks, weak boundaries, unsafe applies
- CI drift: version mismatch, unreviewed applies, missing artifacts
- compliance gate gaps: missing policies/approvals/audit controls

## 3) Load only the relevant reference file(s)
```

</details>
