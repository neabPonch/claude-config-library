---
name: EstrellaXD__Auto_Bangumi
source: https://github.com/EstrellaXD/Auto_Bangumi/blob/717ad11f7fad572ee8fe8ffe7edfe68bde9624c8/CLAUDE.md
repo: EstrellaXD/Auto_Bangumi
kind: claude-md
stars: 8079
last_pushed: 2026-04-19T11:10:30Z
license: mit
score: 9
domains: [backend-api, web-frontend, automation-tools]
tags: [python, vue3, fastapi, architecture-map, workflow-instructions]
curated: 2026-06-14
curated_by: config-scout
---

# EstrellaXD/Auto_Bangumi — claude-md

**Why it's worth keeping:** Includes a highly effective visual architecture tree and explicit instructions for the manual database migration process which prevents LLM hallucinations. The use of specific tooling commands (uv, pnpm) ensures environment-agnostic execution.

**Summary:** Provides comprehensive technical guidance including full development command sets, directory structures, and specific operational workflows.

**Source credibility:** High; project is well-established with over 8k stars and recent activity.

**Recency:** 

**Source:** [EstrellaXD/Auto_Bangumi/CLAUDE.md](https://github.com/EstrellaXD/Auto_Bangumi/blob/717ad11f7fad572ee8fe8ffe7edfe68bde9624c8/CLAUDE.md) · 8079★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AutoBangumi is an RSS-based automatic anime downloading and organization tool. It monitors RSS feeds from anime torrent sites (Mikan, DMHY, Nyaa), downloads episodes via qBittorrent, and organizes files into a Plex/Jellyfin-compatible directory structure with automatic renaming.

## Development Commands

### Backend (Python)

```bash
# Install dependencies
cd backend && uv sync

# Install with dev tools
cd backend && uv sync --group dev

# Run development server (port 7892, API docs at /docs)
cd backend/src && uv run python main.py

# Run tests
cd backend && uv run pytest
cd backend && uv run pytest src/test/test_xxx.py -v  # run specific test

# Linting and formatting
cd backend && uv run ruff check src
cd backend && uv run black src

# Add a dependency
cd backend && uv add <package>

# Add a dev dependency
cd backend && uv add --group dev <package>
```

### Frontend (Vue 3 + TypeScript)

```bash
cd webui

# Install dependencies (uses pnpm, not npm)
pnpm install

# Development server (port 5173)
pnpm dev

# Build for production
pnpm build

# Typ
```

</details>
