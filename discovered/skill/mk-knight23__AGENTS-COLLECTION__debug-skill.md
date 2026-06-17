---
name: mk-knight23__AGENTS-COLLECTION__debug-skill
source: https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/debug-SKILL.md
repo: mk-knight23/AGENTS-COLLECTION
kind: skill
stars: 72
last_pushed: 2026-04-16T07:24:00Z
license: unknown
score: 8
domains: [devops, containerization, ai-agents]
tags: [docker, debugging, persistence, environment-variables]
curated: 2026-06-16
curated_by: config-scout
---

# mk-knight23/AGENTS-COLLECTION — skill

**Why it's worth keeping:** It provides specific, transferable patterns for debugging environment variable injection in interactive containers and ensuring stateful session resumption through precise mount paths.

**Summary:** A highly detailed troubleshooting guide for a containerized agent architecture, covering volume mounts, user permissions, and session persistence.

**Source credibility:** High-quality technical documentation from a frequently updated repository.

**Recency:** Very current (updated within last 2 months).

**Source:** [mk-knight23/AGENTS-COLLECTION/DOCS/.CLAUDE/debug-SKILL.md](https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/debug-SKILL.md) · 72★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: debug
description: Debug container agent issues. Use when things aren't working, container fails, authentication problems, or to understand how the container system works. Covers logs, environment variables, mounts, and common issues.
---

# NanoClaw Container Debugging

This guide covers debugging the containerized agent execution system.

## Architecture Overview

```
Host (macOS)                          Container (Linux VM)
─────────────────────────────────────────────────────────────
src/container-runner.ts               container/agent-runner/
    │                                      │
    │ spawns container                      │ runs Claude Agent SDK
    │ with volume mounts                   │ with MCP servers
    │                                      │
    ├── data/env/env ──────────────> /workspace/env-dir/env
    ├── groups/{folder} ───────────> /workspace/group
    ├── data/ipc/{folder} ────────> /workspace/ipc
    ├── data/sessions/{folder}/.claude/ ──> /home/node/.claude/ (isolated per-group)
    └── (main only) project root ──> /workspace/project
```

**Important:** The container runs as user `node` with `HOME=/home/node`. Session files must be mounted
```

</details>
