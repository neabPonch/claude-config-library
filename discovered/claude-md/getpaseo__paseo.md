---
name: getpaseo__paseo
source: https://github.com/getpaseo/paseo/blob/71b5c35d9b3c7ae96ec01bc3f59e0da9df7b72d0/CLAUDE.md
repo: getpaseo/paseo
kind: claude-md
stars: 8615
last_pushed: 2026-06-15T06:23:04Z
license: other
score: 9
domains: [monorepo, mobile-app, cli-tools, system-architecture]
tags: [monorepo-mapping, knowledge-management, safety-guardrails, developer-experience]
curated: 2026-06-15
curated_by: config-scout
---

# getpaseo/paseo — claude-md

**Why it's worth keeping:** The distinction between code-level facts vs. system/process docs is an elite meta-instruction; the 'Critical Rules' section provides essential guardrails to prevent agent self-sabotage during dev tasks.

**Summary:** Provides a high-density mapping of a monorepo structure and establishes a strict methodology for how documentation should be used and updated.

**Source credibility:** High (8.6k stars, very active repository).

**Recency:** Very recent and highly relevant to current Claude Code capabilities.

**Source:** [getpaseo/paseo/CLAUDE.md](https://github.com/getpaseo/paseo/blob/71b5c35d9b3c7ae96ec01bc3f59e0da9df7b72d0/CLAUDE.md) · 8615★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Paseo is a mobile app for monitoring and controlling your local AI coding agents from anywhere. Your dev environment, in your pocket. Connects directly to your actual development environment — your code stays on your machine.

**Supported agents:** Claude Code, Codex, GitHub Copilot, OpenCode, and Pi.

## Repository map

This is an npm workspace monorepo:

- `packages/server` — Daemon: agent lifecycle, WebSocket API, MCP server
- `packages/app` — Mobile + web client (Expo)
- `packages/cli` — Docker-style CLI (`paseo run/ls/logs/wait`)
- `packages/relay` — E2E encrypted relay for remote access
- `packages/desktop` — Electron desktop wrapper
- `packages/website` — Marketing site (paseo.sh)

## Docs

`docs/` is the source of truth for system-level and process-level knowledge. **"The docs", "check the docs", or "check the X docs" always mean this directory — not the web.** Look here before fetching anything online; the docs capture gotchas and conventions you cannot derive from the code or external sources.

At the start of non-trivial work, list `docs/` and skim anything relevant to the task. When you learn something meta worth preserving — a gotcha, a convention, a workf
```

</details>
