---
name: zhenruyan__postgrebase
source: https://github.com/zhenruyan/postgrebase/blob/536e0c5f01305a464024e03db42f4b2b4c3ef11a/CLAUDE.md
repo: zhenruyan/postgrebase
kind: claude-md
stars: 80
last_pushed: 2026-05-05T11:40:32Z
license: mit
score: 7
domains: [backend-api, go]
tags: [go, sql, cli]
curated: 2026-06-15
curated_by: config-scout
---

# zhenruyan/postgrebase — claude-md

**Why it's worth keeping:** Provides precise DSN connection string templates and highlights critical directory constraints like the mandatory /vendor folder.

**Summary:** Detailed build and execution instructions including specific CLI flags for various database drivers.

**Source credibility:** Decent niche popularity with active maintenance indicated by recent pushes.

**Recency:** Current, providing relevant Go-based backend instructions.

**Source:** [zhenruyan/postgrebase/CLAUDE.md](https://github.com/zhenruyan/postgrebase/blob/536e0c5f01305a464024e03db42f4b2b4c3ef11a/CLAUDE.md) · 80★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PocketBase (Enterprise-Ready PostgreSQL & MySQL Fork)

## Overview
This project is a high-performance, enterprise-ready fork of [PocketBase](https://pocketbase.io). The core storage engine has been replaced with **PostgreSQL** and **MySQL** to handle high-concurrency, clustered, and complex data environments that SQLite cannot support. It features a hybrid caching mechanism that supports both **Redis** (for clusters) and **In-Memory** (for standalone) caching.

## Tech Stack
- **Language:** Go (1.18+)
- **Database Driver:** `github.com/lib/pq` (PostgreSQL), `github.com/go-sql-driver/mysql` (MySQL)
- **Caching:** `github.com/redis/go-redis/v9` (Redis) / Built-in memory store
- **Architecture:** Modified PocketBase `core`, `daos`, `models`, `apis` for SQL dialect compatibility and hybrid caching.

## Project Structure
- `build/`: Main server entry point (`main.go`).
- `core/`: Application logic. `db_postgresql.go` handles DSN parsing; `base.go` contains hybrid cache initialization.
- `vendor/`: **Must be preserved.** Contains all dependencies for offline/strict environment builds.
- `pocketbase.go`: Main package file; handles command-line flags like `--dataDsn` and `--redisDsn`.

#
```

</details>
