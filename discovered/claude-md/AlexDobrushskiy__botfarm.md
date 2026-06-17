---
name: AlexDobrushskiy__botfarm
source: https://github.com/AlexDobrushskiy/botfarm/blob/775a439cb5bd248da2933c0047ab827fb4342f91/CLAUDE.md
repo: AlexDobrushskiy/botfarm
kind: claude-md
stars: 14
last_pushed: 2026-04-16T23:34:06Z
license: other
score: 9
domains: [cli-tools, agents-ai, automation]
tags: [architecture-mapping, agentic-workflow, design-principles]
curated: 2026-06-16
curated_by: config-scout
---

# AlexDobrushskiy/botfarm — claude-md

**Why it's worth keeping:** The 'Code over agents' design principle is a masterclass in efficient prompting, ensuring the agent uses deterministic code instead of reasoning for trivial tasks.

**Summary:** Provides highly structured architectural context, runtime state mapping, and specialized task workflows for an autonomous agent system.

**Source credibility:** Small-scale but highly sophisticated tool with recent maintenance (2 months ago).

**Recency:** Extremely current; includes modern patterns like MCP config injection and specific Claude CLI usage.

**Source:** [AlexDobrushskiy/botfarm/CLAUDE.md](https://github.com/AlexDobrushskiy/botfarm/blob/775a439cb5bd248da2933c0047ab827fb4342f91/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Context
- Botfarm: autonomous ticket dispatcher for AI coding agents (supports Linear and Jira)
- Pure Python CLI project — optional web dashboard, no run.sh/stop.sh
- Database schema has versioned migrations in `db.py` (current: v5)
- This file primarily covers the implementer workflow. Reviewer and review-addresser agents receive instructions via prompt.

## Architecture
Modules under `botfarm/`:
- `cli.py` — Click/Rich CLI (status, history, limits, init, run)
- `config.py` — YAML config loading with `${ENV_VAR}` expansion and validation
- `supervisor.py` — Main loop: poll Linear, dispatch workers via multiprocessing, manage timeouts, crash recovery
- `worker.py` — Stage pipeline: implement → review → fix → pr_checks → merge (iterates review/CI fix loops); also runs `qa` pipeline (single `qa` stage)
- `slots.py` — Slot lifecycle & JSON state persistence (free/busy/paused_limit/failed/completed_pending_cleanup)
- `db.py` — SQLite (sync, WAL mode) for tasks, stage_runs, usage_snapshots, task_events
- `bugtracker/` — Abstract bugtracker interfaces, adapters (Linear, Jira), and factory
- `usage.py` — Anthropic usage API polling, threshold-based dispatch pausin
```

</details>
