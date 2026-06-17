---
name: NVIDIA__OpenShell__skill
source: https://github.com/NVIDIA/OpenShell/blob/ec197a43ef349e36c3fff04e9aaea9599fb83b31/.agents/skills/create-spike/SKILL.md
repo: NVIDIA/OpenShell
kind: skill
stars: 7098
last_pushed: 2026-06-13T21:56:04Z
license: apache-2.0
score: 9
domains: [agents-ai, devops, security, cli-tools]
tags: [spike, investigation, github-automation]
curated: 2026-06-15
curated_by: config-scout
---

# NVIDIA/OpenShell — skill

**Why it's worth keeping:** It demonstrates elite orchestration via a specialized 'principal-engineer' persona and includes highly transferable research checklists like LSM/security impact and architecture mapping.

**Summary:** A sophisticated workflow that uses an investigative sub-agent to transform vague user requirements into structured technical 'spikes' (GitHub issues).

**Source credibility:** High; sourced from NVIDIA's OpenShell project which focuses on autonomous agent runtimes.

**Recency:** Highly current, utilizing advanced sub-agent orchestration patterns essential for Claude Code.

**Source:** [NVIDIA/OpenShell/.agents/skills/create-spike/SKILL.md](https://github.com/NVIDIA/OpenShell/blob/ec197a43ef349e36c3fff04e9aaea9599fb83b31/.agents/skills/create-spike/SKILL.md) · 7098★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: create-spike
description: Investigate a plain-language problem description by deeply exploring the codebase, then create a structured GitHub issue with technical findings. Prequel to build-from-issue — maps vague ideas to concrete, buildable issues. Trigger keywords - spike, investigate, explore, research issue, technical investigation, create spike, new spike, feasibility, codebase exploration.
---

# Create Spike

Investigate a problem, map it to the codebase, and produce a structured GitHub issue ready for `build-from-issue`.

A **spike** is an exploratory investigation. The user has a vague idea — a feature they want, a bug they've noticed, a performance concern — but hasn't mapped it to code, assessed feasibility, or structured it as a buildable issue. This skill does that mapping.

## Prerequisites

- The `gh` CLI must be authenticated (`gh auth status`)
- You must be in a git repository with a GitHub remote

## Workflow Overview

```
User describes a problem
  │
  ├─ Step 1: Gather the problem statement
  │   └─ Ask ONE round of clarifying questions if genuinely needed
  │
  ├─ Step 2: Deep codebase investigation via principal-engineer-reviewer
  │   └─ Map the pro
```

</details>
