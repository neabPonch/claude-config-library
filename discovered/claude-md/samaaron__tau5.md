---
name: samaaron__tau5
source: https://github.com/samaaron/tau5/blob/720e46deb95a55649d2fd0ffcbffd334b40a346f/CLAUDE.md
repo: samaaron/tau5
kind: claude-md
stars: 202
last_pushed: 2026-02-06T11:48:34Z
license: mit
score: 9
domains: [elixir, phoenix-liveview, systems-programming, mcp-integration]
tags: [agent-workflows, debugging-patterns, build-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# samaaron/tau5 — claude-md

**Why it's worth keeping:** It includes 'Agent Workflows' and specific code snippets for state inspection/debugging that teach the agent how to verify its own work. The strict constraints on build tools (no npm) prevent common AI-driven environment corruption.

**Summary:** A sophisticated technical manual that guides an AI through a multi-layered stack (Elixir/Qt) while providing explicit protocols for using specialized MCP servers.

**Source credibility:** High; part of a notable 200+ star open-source project specializing in creative coding.

**Recency:** Very current, specifically optimized for the MCP/Agentic workflow era.

**Source:** [samaaron/tau5/CLAUDE.md](https://github.com/samaaron/tau5/blob/720e46deb95a55649d2fd0ffcbffd334b40a346f/CLAUDE.md) · 202★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md — Tau5 Development Guidelines

## Project Overview
- Tau5 is a collaborative creative coding platform for music, visuals, and live interactive art.
- Built on the **BEAM VM** with Elixir/Phoenix for the server and **Qt/C++** hosting a full Chromium browser for the GUI.

## Tau5 has two build modes
1. Dev - Development mode - contains built-in dev tools and runs Phoenix in dev mode from source with auto-compile and asset-building enabled by deafult.
2. Release - No dev tools, Phoenix running in production mode from a mix release.

## Deployment Modes (TAU5_MODE)
Tau5 has three deployment modes that control routing and features:
1. **`:gui`** - Desktop app mode. The full app - Qt Chromium Browser + Elixir Phoenix Server + NIFs. Routes `/` to `/app` (MainLive LiveView)
2. **`:node`** - Headless server mode (default). Qt CLI + Elixir Phoenix Server + NIFs. Routes `/` to `/app` (MainLive LiveView)
3. **`:central`** - Live web mode. Elixir Phoenix Server only. Routes `/` to a special WebGL shader landing page (CentralController). Used for central/hosted deployments (e.g., tau5.live)

## Environment
- **Default assumption**: development mode (`MIX_ENV=dev`).
- **Release mode**
```

</details>
