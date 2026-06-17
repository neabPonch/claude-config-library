---
name: eddielueng__hermes-agent-zh__skill-backup
source: https://github.com/eddielueng/hermes-agent-zh/blob/69a4d4d9165afa4cbc9f6eb6657963ee9e180148/skills/autonomous-ai-agents/claude-code/SKILL.md.backup
repo: eddielueng/hermes-agent-zh
kind: skill
stars: 1
last_pushed: 2026-04-23T15:34:43Z
license: mit
score: 9
domains: [cli-tools, agents-ai, automation]
tags: [claude-code, tmux, orchestration, automation]
curated: 2026-06-16
curated_by: config-scout
---

# eddielueng/hermes-agent-zh — skill

**Why it's worth keeping:** Includes highly specific 'gold' sequences for using tmux to bypass CLI permission dialogs and provides detailed technical specs for JSON output/streaming parsing.

**Summary:** Provides sophisticated orchestration patterns for integrating Claude Code into automated pipelines via non-interactive print mode and interactive tmux sessions.

**Source credibility:** Low star count, but the content demonstrates deep, specialized knowledge of terminal PTY interaction and Claude Code internals.

**Recency:** Very current; aligns with recent v2.x features like print mode and structured JSON output.

**Source:** [eddielueng/hermes-agent-zh/skills/autonomous-ai-agents/claude-code/SKILL.md.backup](https://github.com/eddielueng/hermes-agent-zh/blob/69a4d4d9165afa4cbc9f6eb6657963ee9e180148/skills/autonomous-ai-agents/claude-code/SKILL.md.backup) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: claude-code
description: Delegate coding tasks to Claude Code (Anthropic's CLI agent). Use for building features, refactoring, PR reviews, and iterative coding. Requires the claude CLI installed.
version: 2.2.0
author: Hermes Agent + Teknium
license: MIT
metadata:
  hermes:
    tags: [Coding-Agent, Claude, Anthropic, Code-Review, Refactoring, PTY, Automation]
    related_skills: [codex, hermes-agent, opencode]
---

# Claude Code — Hermes Orchestration Guide

Delegate coding tasks to [Claude Code](https://code.claude.com/docs/en/cli-reference) (Anthropic's autonomous coding agent CLI) via the Hermes terminal. Claude Code v2.x can read files, write code, run shell commands, spawn subagents, and manage git workflows autonomously.

## Prerequisites

- **Install:** `npm install -g @anthropic-ai/claude-code`
- **Auth:** run `claude` once to log in (browser OAuth for Pro/Max, or set `ANTHROPIC_API_KEY`)
- **Console auth:** `claude auth login --console` for API key billing
- **SSO auth:** `claude auth login --sso` for Enterprise
- **Check status:** `claude auth status` (JSON) or `claude auth status --text` (human-readable)
- **Health check:** `claude doctor` — checks auto-updater
```

</details>
