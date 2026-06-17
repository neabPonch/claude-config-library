---
name: stellarlinkco__myclaude__skill
source: https://github.com/stellarlinkco/myclaude/blob/f2e75c1263a2d5f09cdc4bb3dfe3635c635ff296/skills/do/SKILL.md
repo: stellarlinkco/myclaude
kind: skill
stars: 2697
last_pushed: 2026-05-04T04:25:57Z
license: agpl-3.0
score: 9
domains: [agents-ai, software-engineering, cli-tools]
tags: [orchestrator, workflow, parallel-execution]
curated: 2026-06-17
curated_by: config-scout
---

# stellarlinkco/myclaude — skill

**Why it's worth keeping:** It employs advanced patterns like parallelized codebase exploration, deferred worktree isolation for safety, and domain-specific skill injection to maintain high implementation standards.

**Summary:** A professional-grade orchestration skill that transforms Claude into a structured feature development engine via a rigorous five-phase lifecycle.

**Source credibility:** High; derived from a highly starred (2697) specialized multi-agent orchestration repository.

**Recency:** Highly current; utilizes modern patterns for agentic task management and environment isolation.

**Source:** [stellarlinkco/myclaude/skills/do/SKILL.md](https://github.com/stellarlinkco/myclaude/blob/f2e75c1263a2d5f09cdc4bb3dfe3635c635ff296/skills/do/SKILL.md) · 2697★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: do
description: This skill should be used for structured feature development with codebase understanding. Triggers on /do command. Provides a 5-phase workflow (Understand, Clarify, Design, Implement, Complete) using codeagent-wrapper to orchestrate code-explorer, code-architect, code-reviewer, and develop agents in parallel.
allowed-tools: ["Bash(python3:*/.claude/skills/do/scripts/setup-do.py*)", "Bash(python3:*/.claude/skills/do/scripts/task.py*)"]
---

# do - Feature Development Orchestrator

An orchestrator for systematic feature development. Invoke agents via `codeagent-wrapper`, never write code directly.

## Loop Initialization (REQUIRED)

When triggered via `/do <task>`, initialize the task directory immediately without asking about worktree:

```bash
python3 "$HOME/.claude/skills/do/scripts/setup-do.py" "<task description>"
```

This creates a task directory under `.claude/do-tasks/` with:
- `task.md`: Single file containing YAML frontmatter (metadata) + Markdown body (requirements/context)

**Worktree decision is deferred until Phase 4 (Implement).** Phases 1-3 are read-only and do not require worktree isolation.

## Task Directory Management

Use `task.py` to m
```

</details>
