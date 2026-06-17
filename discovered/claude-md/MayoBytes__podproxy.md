---
name: MayoBytes__podproxy
source: https://github.com/MayoBytes/podproxy/blob/8a8a5c6b2512619e60e1393bbf4aa19f90f95486/CLAUDE.md
repo: MayoBytes/podproxy
kind: claude-md
stars: 2
last_pushed: 2026-04-26T18:04:49Z
license: gpl-3.0
score: 9
domains: [backend, systems]
tags: [go, caching, proxy]
curated: 2026-06-16
curated_by: config-scout
---

# MayoBytes/podproxy — claude-md

**Why it's worth keeping:** The 'Key Implementation Details' section documents subtle concurrency patterns and I/O strategies that prevent an AI from introducing regressions. It also explicitly maps internal data states to the filesystem structure.

**Summary:** Provides high-density technical context including architecture diagrams, API specs, and critical low-level implementation nuances.

**Source credibility:** A niche personal project with steady recent activity.

**Recency:** Extremely current, based on a repository updated within the last two months.

**Source:** [MayoBytes/podproxy/CLAUDE.md](https://github.com/MayoBytes/podproxy/blob/8a8a5c6b2512619e60e1393bbf4aa19f90f95486/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# podproxy — CLAUDE.md

## Project Overview

A self-hosted Go podcast caching proxy. Podcast apps add a proxied RSS URL; the server rewrites enclosure URLs to point at itself, then stream-caches episodes to disk on first play. Future plays (and other devices) are served from local cache.

## Architecture

```
Podcast App → /feeds/:id.rss       → rewritten RSS with proxy URLs
Podcast App → /episodes/:feed/:ep  → write-through stream cache
```

**Key subsystems:**

| Package | Role |
|---|---|
| `internal/config` | YAML config loading with defaults |
| `internal/db` | SQLite CRUD for feeds and episodes |
| `internal/feed` | RSS fetching/parsing, background poller, prefetch worker pool |
| `internal/proxy` | Episode handler: cache hit → `http.ServeContent`; miss → `io.TeeReader` stream-while-caching |
| `internal/api` | REST API handlers |
| `internal/backup` | On-demand and scheduled database backups via `VACUUM INTO` |
| `internal/ui` | HTMX web UI with embedded HTML templates |

## Data Model

Two SQLite tables: `feeds` and `episodes`. Episode `cache_status` is one of: `none`, `in_progress`, `cached`, `failed`. Feeds have an `auto_prefetch` boolean flag.

Episode files live at `{ca
```

</details>
