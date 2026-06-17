---
name: vishalsachdev__claude-skills__skill
source: https://github.com/vishalsachdev/claude-skills/blob/f769feeab171c82a41d50fa7e591aa855d9bd530/agentic-validators/SKILL.md
repo: vishalsachdev/claude-skills
kind: skill
stars: 2
last_pushed: 2026-01-24T16:38:05Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, devops]
tags: [validation, hooks, automation, reliability]
curated: 2026-06-15
curated_by: config-scout
---

# vishalsachdev/claude-skills — skill

**Why it's worth keeping:** The distinction between 'post-tool-use' (fast, local) and 'stop-hook' (slow, global) gates is a highly transferable architectural pattern for building reliable agentic workflows. The patterns for handling parallel subagents through validator aggregation are also valuable.

**Summary:** Provides a strategic framework for implementing validation hooks (per-file vs. repo-wide) to ensure AI-generated code is deterministic and safe. It distinguishes between immediate post-tool feedback loops and final exit criteria.

**Source credibility:** Low social proof (2 stars), but the content reflects sophisticated, structured engineering thought rather than generic AI filler.

**Recency:** Current; aligns with modern trends in agentic reliability and tool-use loops.

**Source:** [vishalsachdev/claude-skills/agentic-validators/SKILL.md](https://github.com/vishalsachdev/claude-skills/blob/f769feeab171c82a41d50fa7e591aa855d9bd530/agentic-validators/SKILL.md) · 2★

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
