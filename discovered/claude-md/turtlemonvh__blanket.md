---
name: turtlemonvh__blanket
source: https://github.com/turtlemonvh/blanket/blob/91b44faad685a2c60da489081a713ed8b2b475b1/CLAUDE.md
repo: turtlemonvh/blanket
kind: claude-md
stars: 6
last_pushed: 2026-05-04T01:49:29Z
license: unknown
score: 9
domains: [backend-api, cli-tools, go]
tags: [go, docker, infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# turtlemonvh/blanket — claude-md

**Why it's worth keeping:** The 'Gotchas' section is exceptional for preempting common failure modes like Docker volume shadowing and database locks; the directory map provides vital spatial awareness.

**Summary:** Provides deep architectural context alongside explicit build instructions and operational friction points.

**Source credibility:** Small, focused project with recent maintenance activity.

**Recency:** Very current (mentions Go 1.23).

**Source:** [turtlemonvh/blanket/CLAUDE.md](https://github.com/turtlemonvh/blanket/blob/91b44faad685a2c60da489081a713ed8b2b475b1/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude (or any agent) working in this repo. The README is
the user-facing entrypoint; this file captures the conventions and
gotchas that save a cold session from relearning them.

## What blanket is

A single Go binary that wraps long-running command-line tasks behind a
REST API + HTMX web UI + CLI. Tasks are defined as TOML files; workers
claim them off a queue and shell out. Server and worker are the same
binary invoked with different subcommands.

## Tech stack

- **Go 1.23** (pinned in Dockerfile), `go.mod`-managed.
- **BoltDB** for storage (`lib/bolt`); internal queue abstraction at
  `lib/queue` + `lib/bolt/queue.go`.
- **Gin** for HTTP routing; `//go:embed` bakes the UI into the binary.
- **Server-rendered Go templates + htmx** under `server/ui_next/` —
  there is no SPA, no JS build step.
- **Playwright (TS)** for the browser journey suite under `tests/e2e/`.

## Where things live

- `server/` — HTTP handlers, UI rendering, embedded assets.
  Handler files are split by resource: `serve_tasks.go`, `serve_workers.go`,
  `serve_task_types.go`, `serve_config.go`, `ui_next.go`.
- `worker/` — claim loop, task exec, daemonization.
- `tasks/` — `Task` + `
```

</details>
