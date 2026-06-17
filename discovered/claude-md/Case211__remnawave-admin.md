---
name: Case211__remnawave-admin
source: https://github.com/Case211/remnawave-admin/blob/9cacda59376c178a1f13cbbafda312c5e581c35a/CLAUDE.md
repo: Case211/remnawave-admin
kind: claude-md
stars: 223
last_pushed: 2026-06-07T15:50:54Z
license: mit
score: 9
domains: [backend-api, web-frontend, monorepo, security]
tags: [python, fastapi, react, architecture-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# Case211/remnawave-admin — claude-md

**Why it's worth keeping:** It documents critical cross-service logic like data/authentication flows and configuration priority, which prevents the AI from hallucinating incorrect interaction patterns.

**Summary:** A high-density architectural blueprint for a complex monorepo containing a Telegram bot, FastAPI backend, and React frontend.

**Source credibility:** High; 223 stars and active maintenance suggest a well-structured production codebase.

**Recency:** Extremely current; updated within the last month.

**Source:** [Case211/remnawave-admin/CLAUDE.md](https://github.com/Case211/remnawave-admin/blob/9cacda59376c178a1f13cbbafda312c5e581c35a/CLAUDE.md) · 223★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Remnawave Admin is a monorepo containing three integrated components for managing Remnawave VPN panel:

1. **Telegram Bot** (`src/`) - Python/aiogram bot for admin operations
2. **Web Backend** (`web/backend/`) - FastAPI REST API
3. **Web Frontend** (`web/frontend/`) - React + TypeScript SPA

All three share a common PostgreSQL database and use a `shared/` module for reusable code.

## Architecture

### Shared Module (`shared/`)

Critical shared components used by both bot and web backend:

- **`database.py`** - AsyncPG connection pool, all DB operations (users, nodes, hosts, violations, connections, IP metadata)
- **`api_client.py`** - HTTP client for Remnawave Panel API (handles auth, retries, rate limiting)
- **`config_service.py`** - Dynamic configuration (DB-first, then .env fallback)
- **`logger.py`** - Structlog-based logging (JSON output, processor pipeline)
- **`sync.py`** - Background sync service (Panel API → local DB cache)
- **`connection_monitor.py`** - Active connection tracking and stats (used by violation detector)
- **`violation
```

</details>
