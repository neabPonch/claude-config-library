---
name: vishalsachdev__claude-code-skills__skill
source: https://github.com/vishalsachdev/claude-code-skills/blob/3ae6ce09a01eebdf0f23bd7f8ffbe27babe9414e/skills/agentic-validators/SKILL.md
repo: vishalsachdev/claude-code-skills
kind: skill
stars: 4
last_pushed: 2026-05-02T19:32:36Z
license: other
score: 8
domains: [agents-ai, devops, software-engineering]
tags: [validation, automation, testing-strategy]
curated: 2026-06-14
curated_by: config-scout
---

# vishalsachdev/claude-code-skills — skill

**Why it's worth keeping:** The distinction between immediate 'post-tool-use' hooks and broader 'stop' gatekeepers is a high-value architectural pattern for reducing error feedback cycles in agentic workflows.

**Summary:** Provides a strategic framework for implementing multi-stage validation loops (per-file vs. repo-wide) to ensure AI-driven changes are safe and deterministic.

**Source credibility:** Niche repository with recent activity, suggesting it targets an emerging specific use case.

**Recency:** Current; highly relevant to the iterative nature of tools like Claude Code and Aider.

**Source:** [vishalsachdev/claude-code-skills/skills/agentic-validators/SKILL.md](https://github.com/vishalsachdev/claude-code-skills/blob/3ae6ce09a01eebdf0f23bd7f8ffbe27babe9414e/skills/agentic-validators/SKILL.md) · 4★

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
