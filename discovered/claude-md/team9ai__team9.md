---
name: team9ai__team9
source: https://github.com/team9ai/team9/blob/fdc1143e9105e8bc0cc6f17fae5bc825d4c973ce/CLAUDE.md
repo: team9ai/team9
kind: claude-md
stars: 1502
last_pushed: 2026-06-10T08:23:34Z
license: other
score: 9
domains: [fullstack, monorepo, real-time]
tags: [nestjs, react, tauri, drizzle-orm, websockets]
curated: 2026-06-15
curated_by: config-scout
---

# team9ai/team9 — claude-md

**Why it's worth keeping:** Exceptional detail on domain-specific logic like 'long text' truncation and the 'Edition' system, which prevents AI hallucinations. The breakdown of state management layers (Zustand vs TanStack Query) provides clear architectural guardrails.

**Summary:** Comprehensive guide for a complex monorepo featuring backend services (NestJS) and a desktop frontend (Tauri/React). It bridges the gap between code location and business logic rules.

**Source credibility:** High; part of a highly-starred repository with active development.

**Recency:** Very current; utilizes modern full-stack tooling and patterns compatible with today's Claude Code workflows.

**Source:** [team9ai/team9/CLAUDE.md](https://github.com/team9ai/team9/blob/fdc1143e9105e8bc0cc6f17fae5bc825d4c973ce/CLAUDE.md) · 1502★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Team9 is a full-stack instant messaging and team collaboration platform built as a monorepo. The backend uses NestJS with PostgreSQL (Drizzle ORM), while the frontend is a Tauri-based cross-platform desktop app (React + TypeScript) with real-time WebSocket communication via Socket.io.

## Common Commands

### Development

```bash
pnpm dev              # Run server (gateway + im-worker) and client concurrently
pnpm dev:client       # Web frontend only (Vite dev server)
pnpm dev:desktop      # Tauri desktop app (hot reload)
pnpm dev:server       # Gateway service only
pnpm dev:im-worker    # Background IM worker service only
pnpm dev:server:all   # Both gateway and im-worker services
```

> Note: `pnpm dev` and other scripts use Turborepo for task orchestration.
> Build artifacts are cached locally in `.turbo/`. Run `turbo run build`
> directly if you need fine-grained control (e.g., `--filter`, `--dry`).

### Database Operations

```bash
pnpm db:generate      # Generate Drizzle schemas from TypeScript
pnpm db:migrate       # Run pending migrations
```

</details>
