---
name: progressions__shot-server-elixir
source: https://github.com/progressions/shot-server-elixir/blob/801d62abd8305035b4eeb4011ce6682256b81acd/CLAUDE.md
repo: progressions/shot-server-elixir
kind: claude-md
stars: 0
last_pushed: 2026-01-31T16:43:14Z
license: unknown
score: 9
domains: [backend-api, elixir, phoenix]
tags: [api-compatibility, architectural-rules, json-serialization]
curated: 2026-06-15
curated_by: config-scout
---

# progressions/shot-server-elixir — claude-md

**Why it's worth keeping:** Uses 'Correct vs Wrong' code blocks and detailed mapping tables to enforce strict JSON response structures. It proactively defines custom view module patterns that deviate from standard Phoenix defaults to ensure API compatibility.

**Summary:** Provides precise architectural constraints for a Phoenix API designed as a drop-in replacement for a Rails backend sharing a database.

**Source credibility:** Low star count, but the level of specific, practical detail suggests a production-grade technical requirement document.

**Recency:** Very current; utilizes modern Phoenix 1.8 and highly actionable development workflows.

**Source:** [progressions/shot-server-elixir/CLAUDE.md](https://github.com/progressions/shot-server-elixir/blob/801d62abd8305035b4eeb4011ce6682256b81acd/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Shot Elixir Phoenix API

This Phoenix API replicates the Rails shot-server API endpoints using the same PostgreSQL database.

## Git Workflow

**Never commit directly to main/master.** Always create a feature branch and make a pull request. Wait for CI to pass before merging.

## Project Overview

This is a Phoenix 1.8 API application that provides identical endpoints to the Rails shot-server, sharing the same database (shot_counter_local). It's designed to be a drop-in replacement for the Rails API with full compatibility.

## Architecture

### Core Technologies
- **Phoenix 1.8** - Web framework
- **PostgreSQL** - Shared database with Rails app
- **Guardian** - JWT authentication (Devise equivalent)
- **Bcrypt** - Password hashing
- **CORS Plug** - Cross-origin request handling
- **Phoenix Channels** - WebSocket support (Action Cable equivalent)

### Database
Uses the existing `shot_counter_local` PostgreSQL database with UUID primary keys.

**Local Development:**
- Development: Shares `shot_counter_local` with Rails
- Test: Shares `shot_server_test` with Rails (Rails must set up schema first)

**Test Database Setup:**
The test database schema comes from Rails. For C
```

</details>
