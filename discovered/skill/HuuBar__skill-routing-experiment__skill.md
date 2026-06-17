---
name: HuuBar__skill-routing-experiment__skill
source: https://github.com/HuuBar/skill-routing-experiment/blob/0731f842467bc34c43e7ca68860c1903da2c4b5a/unified_skills/vishal/agentic-validators/SKILL.md
repo: HuuBar/skill-routing-experiment
kind: skill
stars: 0
last_pushed: 2026-04-21T23:49:44Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, devops]
tags: [validation, automation, guardrails, agentic-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# HuuBar/skill-routing-experiment — skill

**Why it's worth keeping:** The architectural distinction between fast per-file 'post-tool' validators and global 'stop-hook' gates is a high-value strategy for agentic workflows.

**Summary:** Provides a framework for implementing automated validation hooks to ensure agent-generated code remains deterministic and safe.

**Source credibility:** Low visibility (0 stars) and experimental status, but provides sophisticated structural thinking.

**Recency:** Highly current; addresses the specific need for guardrails in non-deterministic CLI agent workflows.

**Source:** [HuuBar/skill-routing-experiment/unified_skills/vishal/agentic-validators/SKILL.md](https://github.com/HuuBar/skill-routing-experiment/blob/0731f842467bc34c43e7ca68860c1903da2c4b5a/unified_skills/vishal/agentic-validators/SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: agentic-validators
description: Design and install validation hooks for coding agents (e.g., Claude Code) to make AI changes safer and more deterministic. Use when you want post-tool-use or stop hooks, automated tests/linters/formatters, parallel subagents with per-file validation, or a repeatable “agent pipeline” with audit logs.
license: MIT
metadata:
  author: Vishal Sachdev + Pip
  version: "0.1.0"
  tags: "agents hooks validation testing linting formatting ci"
compatibility: Works in repos on macOS/Linux with bash. Assumes a CLI coding agent that supports hooks (Claude Code-style) and common tooling (git, ripgrep, node/python toolchains).
---

# Agentic Validators

## Goal
Turn “agent wrote code” into “agent wrote code **and** the change is validated automatically.”

This skill helps you:
- choose the right validation strategy (per-file vs repo-wide)
- implement **post-tool-use** and **stop** hooks
- create **narrow validators** (fast, deterministic checks)
- structure work so multiple agents can run in parallel without losing correctness

## Mental model
- **Agents are non-deterministic; validators are deterministic.**
- **Context is fragile; validation + logs are d
```

</details>
