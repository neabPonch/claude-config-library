---
name: FulAppiOS__Agent-Quest
source: https://github.com/FulAppiOS/Agent-Quest/blob/010c791207c9e5670f07d0fbca3a62f3d1eb0fa7/CLAUDE.md
repo: FulAppiOS/Agent-Quest
kind: claude-md
stars: 77
last_pushed: 2026-06-12T08:04:16Z
license: mit
score: 9
domains: [web-frontend, backend-api, real-time-visualization, developer-tools]
tags: [monorepo, websocket, architecture, domain-modeling]
curated: 2026-06-15
curated_by: config-scout
---

# FulAppiOS/Agent-Quest — claude-md

**Why it's worth keeping:** The explicit 'Ports' section prevents environment conflicts by banning common defaults, and the 'Key Type' breakdown provides essential domain context for the central data model.

**Summary:** Provides a deep architectural blueprint of a real-time monitoring system including data flow from file logs to WebSocket.

**Source credibility:** High-quality technical documentation in an active, specialized project.

**Recency:** Very current; utilizes modern technologies like React 19 and specific Claude Code integrations.

**Source:** [FulAppiOS/Agent-Quest/CLAUDE.md](https://github.com/FulAppiOS/Agent-Quest/blob/010c791207c9e5670f07d0fbca3a62f3d1eb0fa7/CLAUDE.md) · 77★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Agent Quest is a browser-based monitoring dashboard that visualizes active Claude Code and Codex agent sessions as fantasy heroes in a 2D WoW-style village. Each agent is represented as a hero character that walks between buildings corresponding to its current activity (Read → Library, Edit → Forge, Bash → Arena, etc.).

## Architecture

Two-process monorepo:

- **server/** — Bun + Hono backend. Two providers run in parallel: `ClaudeProvider` auto-discovers every `~/.claude*` directory with a `projects/` subdir (e.g. `~/.claude`, `~/.claude-work`, `~/.claude-personale`); `CodexProvider` watches `~/.codex/sessions/` for Codex rollout files. Both poll their session logs every 2-3s, parse events into `AgentState` objects, push updates over native Bun WebSocket. Each `AgentState` carries its `configDir` and a `source` field (`'claude' | 'codex'`) so the UI can distinguish installations and providers. Optional Hono endpoint receives Claude Code `postToolUse` hooks for lower-latency events — **Claude Code only**; Codex doesn't expose hooks. `SessionReg
```

</details>
