---
name: andrewhollamon__mcb_api
source: https://github.com/andrewhollamon/mcb_api/blob/624809605939cb732c90f4acc58fb9cd6e6455c1/CLAUDE.md
repo: andrewhollamon/mcb_api
kind: claude-md
stars: 0
last_pushed: 2026-03-03T15:08:26Z
license: unknown
score: 8
domains: [backend, distributed-systems, go]
tags: [golang, postgresql, architecture, api]
curated: 2026-06-17
curated_by: config-scout
---

# andrewhollamon/mcb_api — claude-md

**Why it's worth keeping:** It explains the 'why' behind architectural decisions (like partitioning and worker thread logic) which is crucial for AI reasoning about state. It also includes specific orchestration commands for database setup/migrations.

**Summary:** Provides a high-level mental model of a multi-layered Go system featuring eventual consistency between an in-memory store and a partitioned PostgreSQL database.

**Source credibility:** Low star count, but likely a high-quality technical interview or engineering prototype.

**Recency:** Extremely current; mentions Go 1.24 (released Feb 2025).

**Source:** [andrewhollamon/mcb_api/CLAUDE.md](https://github.com/andrewhollamon/mcb_api/blob/624809605939cb732c90f4acc58fb9cd6e6455c1/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Development Commands

### Environment

The development environment is MacOS on AppleSilicon.

The console is `zsh`, though the default bash tool is available.

### Building and Running
- Build the API server: `go build -o bin/api-server ./cmd/api-server`
- Run the API server: `go run ./cmd/api-server/main.go` (runs on port 8080)
- Test the server: `curl http://localhost:8080/ping` (should return "pong")
- Build the Backend server: `go build -o bin/backend ./cmd/backend`
- Run the API server: `go run ./cmd/backend/main.go` (no webserver)

### Database Setup
- Launch local PostgreSQL docker container: `./database/system/setup_database.sh`
- Setup database and roles: Run `database/system/create_db_and_roles.sql`
- Run migrations: `migrate -source database/migrations -database postgres://localhost:5432/database up`
  - Migration uses the `golang-migrate/migrate` tool, which you can assume is installed

### Testing
- Run tests: `go test ./...`
- Run specific package tests: `go test ./internal/memorystore`

## Architecture Overview

This is a "Million Checkboxes"
```

</details>
