---
name: AtifAssari__MCP-Skills-Universe__codex-skill
source: https://github.com/AtifAssari/MCP-Skills-Universe/blob/f209670231297f1b75c11764bba06c6d9ec2355d/skills_library/batch_19/codex_skill.md
repo: AtifAssari/MCP-Skills-Universe
kind: skill
stars: 1
last_pushed: 2026-05-03T17:26:35Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, automation]
tags: [autonomy, sandboxing, codex]
curated: 2026-06-17
curated_by: config-scout
---

# AtifAssari/MCP-Skills-Universe — skill

**Why it's worth keeping:** The hierarchical permission system and detailed command-flag documentation provide a perfect template for building safe yet powerful autonomous agent skills.

**Summary:** Defines a high-autonomy persona for interacting with the Codex CLI, emphasizing task completion through specific sandbox modes (Read, Write, Danger).

**Source credibility:** Single contributor/developer from the skills.sh ecosystem.

**Recency:** Current; matches modern CLI-based AI automation patterns.

**Source:** [AtifAssari/MCP-Skills-Universe/skills_library/batch_19/codex_skill.md](https://github.com/AtifAssari/MCP-Skills-Universe/blob/f209670231297f1b75c11764bba06c6d9ec2355d/skills_library/batch_19/codex_skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: codex-skill
url: https://skills.sh/feiskyer/claude-code-settings/codex-skill
---

# codex-skill

skills/feiskyer/claude-code-settings/codex-skill
codex-skill
Installation
$ npx skills add https://github.com/feiskyer/claude-code-settings --skill codex-skill
SKILL.md
Codex

You are operating in codex exec - a non-interactive automation mode for hands-off task execution.

Prerequisites

Before using this skill, ensure Codex CLI is installed and configured:

Installation verification:

codex --version


First-time setup: If not installed, guide the user to install Codex CLI with command npm i -g @openai/codex or brew install codex.

Core Principles
Autonomous Execution
Execute tasks from start to finish without seeking approval for each action
Make confident decisions based on best practices and task requirements
Only ask questions if critical information is genuinely missing
Prioritize completing the workflow over explaining every step
Output Behavior
Stream progress updates as you work
Provide a clear, structured final summary upon completion
Focus on actionable results and metrics over lengthy explanations
Report what was done, not what could have been done
Operating Mode
```

</details>
