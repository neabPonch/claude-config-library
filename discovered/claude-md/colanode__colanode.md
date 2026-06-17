---
name: colanode__colanode
source: https://github.com/colanode/colanode/blob/d649523637f0f059c936418488165d4a689da27c/CLAUDE.md
repo: colanode/colanode
kind: claude-md
stars: 4914
last_pushed: 2026-04-03T14:23:17Z
license: apache-2.0
score: 9
domains: [monorepo, real-time, fullstack]
tags: [architecture-driven, crdt, local-first, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# colanode/colanode — claude-md

**Why it's worth keeping:** It details critical data flow paths (Write/Read) and specific registry patterns, which prevents the AI from hallucinating incorrect ways to extend the system's core logic.

**Summary:** This config provides an architectural blueprint for a complex local-first monorepo using CRDTs and Yjs.

**Source credibility:** High; highly starred (4.9k+) active open-source project with a clear engineering structure.

**Recency:** Current; includes modern stack details like TanStack Router and recent updates.

**Source:** [colanode/colanode/CLAUDE.md](https://github.com/colanode/colanode/blob/d649523637f0f059c936418488165d4a689da27c/CLAUDE.md) · 4914★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Colanode is an open-source, local-first collaboration platform supporting real-time chat, rich text editing, customizable databases, and file management. It uses a sophisticated CRDT-based architecture (powered by Yjs) to enable offline-first operation with automatic conflict resolution.

## Commands

### Development

```bash
# Install dependencies (also runs postinstall script to generate emoji/icon assets)
npm install
```

Prefer running dev/build/compile/format commands inside the specific app or package directory.

**Note:** Tests exist for `apps/server` and `apps/web` and are run with Vitest. Prefer running tests in the relevant app directory; `npm run test` at the repo root runs the same suites via Turbo.

### Individual App Development

**Server:**

```bash
cd apps/server
cp .env.example .env  # Configure environment variables
npm run dev           # Start server with hot reload

# Start dependencies (Postgres, Redis, Mail server) via Docker Compose
docker compose -f hosting/docker/docker-compose.yaml up -d

# Include MinIO (S3-compatible
```

</details>
