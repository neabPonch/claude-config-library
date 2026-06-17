---
name: FlashHand__rig__rig-crew-skill
source: https://github.com/FlashHand/rig/blob/48d4ed8a3cfbd8495b0ec5c889d40d27cac8cdb6/RIG_CREW_SKILL.md
repo: FlashHand/rig
kind: skill
stars: 7
last_pushed: 2026-05-31T13:35:46Z
license: mit
score: 8
domains: [agents-ai, cli-tools, productivity-workflows]
tags: [multi-agent, obsidian, workflow-orchestration, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# FlashHand/rig — skill

**Why it's worth keeping:** It implements a sophisticated 'file-as-state' architecture where Markdown files serve as a shared, persistent memory/status system for multiple agents. This pattern is highly effective for maintaining context across different agent sessions or executors.

**Summary:** Provides instructions for Claude Code to act as an orchestrator ('Lead') within a file-backed multi-agent workflow using the 'rig crew' CLI and an Obsidian vault.

**Source credibility:** The low star count suggests it is a niche or emerging tool, but the technical depth of the orchestration logic is high.

**Recency:** Current; utilizes modern toolchains like Playwright and contemporary AI model workflows.

**Source:** [FlashHand/rig/RIG_CREW_SKILL.md](https://github.com/FlashHand/rig/blob/48d4ed8a3cfbd8495b0ec5c889d40d27cac8cdb6/RIG_CREW_SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rig-crew
description: >-
  Agent-facing Leader-first multi-agent workflow over an Obsidian vault using
  `rig crew`. Use when the current coding agent should initialize a crew vault,
  refresh a human-readable dashboard, inspect inbox/status, register project
  owners, or coordinate PRD-driven project work through Vault files.
  For frontend testing, default to PRD-scoped Playwright E2E only: do not add
  or run frontend unit/integration tests unless the user or project explicitly
  requires them.
user-invocable: true
disable-model-invocation: false
metadata:
  openclaw:
    requires:
      bins: [rig, node, yarn]
    os: [darwin]
---

# rig-crew

Use this skill when the current coding agent is inside or coordinating an Obsidian Vault that uses `rig crew`: a file-backed, Leader-first agent workflow using Obsidian Markdown as the source of truth.

`rig crew` is primarily for coding agents, not a human-operated daily CLI. The human talks to the active Claude/Codex session; that coding agent should use `rig crew` commands and Vault files to communicate with Crew Lead, coordinate other roles, and stay aware of all agent/todo status.

## Agent Quickstart

```bash
rig crew init
```

</details>
