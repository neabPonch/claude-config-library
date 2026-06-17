---
name: adibirzu__multillm
source: https://github.com/adibirzu/multillm/blob/804dd3392902925fc1c8e782b67af1686c45481e/CLAUDE.md
repo: adibirzu/multillm
kind: claude-md
stars: 1
last_pushed: 2026-05-31T17:50:13Z
license: apache-2.0
score: 8
domains: [agents-ai, cli-tools, orchestration]
tags: [multi-llm, agent-roles, state-management, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# adibirzu/multillm — claude-md

**Why it's worth keeping:** Provides excellent patterns for 'Agent Rosters' and 'Phase-Based Routing' to teach an LLM when to delegate tasks. It also includes structured protocols for session checkpoints and cross-session memory persistence.

**Summary:** Defines a high-level orchestration system where Claude Code interacts with a multi-model gateway using specialized agent roles and shared memory.

**Source credibility:** Low star count (1), but the file is highly sophisticated and reflects recent, active development.

**Recency:** Very current; utilizes modern agentic orchestration concepts suitable for Claude Code.

**Source:** [adibirzu/multillm/CLAUDE.md](https://github.com/adibirzu/multillm/blob/804dd3392902925fc1c8e782b67af1686c45481e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MultiLLM Gateway — Claude Code Instructions

## Overview

MultiLLM is a unified LLM gateway that proxies requests to 16+ backends through a single Anthropic-compatible API. It provides token tracking, cost estimation, shared cross-LLM memory, circuit breakers, health probes, and a real-time dashboard.

**Gateway URL**: `http://localhost:8080`
**Dashboard**: `http://localhost:8080/dashboard`
**Data directory**: `MULTILLM_HOME` or `~/.multillm/` (SQLite DBs, PID file, logs)

## Architecture

```
Claude Code → HTTP requests → FastAPI Gateway (port 8080) → Backend adapters → LLM APIs
                                    ↓
                              SQLite tracking + FTS5 memory + OpenTelemetry
```

- **`multillm/gateway.py`** — Main FastAPI app with all routing logic (inline functions, not adapter registry)
- **`multillm/adapters/`** — Adapter classes per backend (kept in sync with gateway inline functions)
- **`multillm/resilience.py`** — Retry with exponential backoff + per-backend circuit breakers
- **`multillm/health.py`** — Background health probes every 120s, readiness-aware routing
- **`multillm/tracking.py`** — SQLite usage/session tracking + OCI APM via OpenTelemetry
- **`
```

</details>
