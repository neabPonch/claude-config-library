---
name: DenisSergeevitch__repo-task-proof-loop
source: https://github.com/DenisSergeevitch/repo-task-proof-loop/blob/853622144588798dc1b3babc81ed9499328321bf/SKILL.md
repo: DenisSergeevitch/repo-task-proof-loop
kind: skill
stars: 716
last_pushed: 2026-04-01T20:30:40Z
license: apache-2.0
score: 9
domains: [agents-ai, software-engineering, cli-tools, workflows]
tags: [agentic-workflow, verification-loop, structured-tasks, subagents]
curated: 2026-06-14
curated_by: config-scout
---

# DenisSergeevitch/repo-task-proof-loop — skill

**Why it's worth keeping:** The 'fresh verifier' pattern forces validation by a new agent session to prevent self-confirmation bias. It uses structured local artifacts (spec, evidence, verdict) to ensure auditable progress and task state persistence.

**Summary:** A stateful, artifact-driven workflow that manages large tasks through a strict cycle of spec-freezing, building, and fresh-session verification.

**Source credibility:** High; 716 stars indicates significant community value for specialized agentic workflows.

**Recency:** Current; tailored specifically for modern Claude Code and Codex subagent patterns.

**Source:** [DenisSergeevitch/repo-task-proof-loop/SKILL.md](https://github.com/DenisSergeevitch/repo-task-proof-loop/blob/853622144588798dc1b3babc81ed9499328321bf/SKILL.md) · 716★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: repo-task-proof-loop
description: Repo-local workflow skill for large coding tasks. Initializes .agent/tasks/TASK_ID artifacts, installs project-scoped Codex and Claude subagents, updates AGENTS.md plus the repo's Claude guide file with the workflow, and runs a spec-freeze → build → evidence → verify → fix loop with fresh-session verification.
license: Apache-2.0
compatibility: Skills-compatible coding agents. Integrates with Codex and Claude Code project-scoped subagents. Bundled scripts require Python 3.10+.
metadata:
  author: OpenAI
  version: "1.0.0"
---

# Repo Task Proof Loop

Use this skill when the user wants a repeatable, auditable implementation workflow for a non-trivial coding task, especially a feature, refactor, migration, or bug fix that should leave repo-local proof in `.agent/tasks/<TASK_ID>/`.

All task artifacts created by this workflow must stay inside the repository.

When the examples below mention `scripts/task_loop.py`, that path is relative to this skill root. Run it while your shell working directory is inside the target repository.

## What this skill does

1. Initializes a strict repo-local task folder under `.agent/tasks/<TASK_ID>/`
2. Seeds
```

</details>
