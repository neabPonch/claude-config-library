---
name: vemetric__vemetric
source: https://github.com/vemetric/vemetric/blob/44cd835b24c03ff81113d78281a65d460aefcead/CLAUDE.md
repo: vemetric/vemetric
kind: claude-md
stars: 352
last_pushed: 2026-06-01T20:04:36Z
license: agpl-3.0
score: 9
domains: [backend-api, web-frontend, monorepo, data-engineering]
tags: [bun, turborepo, microservices, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# vemetric/vemetric — claude-md

**Why it's worth keeping:** The 'Development Workflow' section successfully explains end-to-end data flow (Hub to Worker to ClickHouse), which is crucial for agents to understand side effects. The clear distinction between the relational and analytics data layers provides essential context for state management and debugging.

**Summary:** Provides a comprehensive architectural map of a complex monorepo, detailing service dependencies and dual-database orchestration.

**Source credibility:** Highly credible; an active, specialized open-source project with significant community interest.

**Recency:** Very current; uses a modern stack (Bun, Hono, TanStack) that aligns perfectly with today's development environments.

**Source:** [vemetric/vemetric/CLAUDE.md](https://github.com/vemetric/vemetric/blob/44cd835b24c03ff81113d78281a65d460aefcead/CLAUDE.md) · 352★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Vemetric is an open-source web and product analytics platform built as a monorepo using Turborepo and bun. It provides real-time analytics, behavior tracking, custom event tracking, and powerful filtering mechanisms.

## Architecture

**Microservices Structure:**

- **app**: Vite SPA + Hono API server (port 4000 in dev) - Single deployable web app + API service
- **hub**: Bun + Hono - Event collection service (`/e` for events, `/i` for identification)
- **worker**: Background job processor using BullMQ and Redis
- **bullboard**: Queue monitoring dashboard
- **health-check**: Service health monitoring

**Data Layer:**

- **PostgreSQL**: User accounts, projects, organizations (via Prisma ORM)
- **ClickHouse**: High-volume analytics data (events, sessions, devices)
- **Redis**: Caching and job queues

## Common Development Commands

```bash
# Development (starts all services except health-check)
bun dev

# Quick Typecheck for all applications
bun run tsc

# Build all applications
bun run build

# Lint all applications
bun lint

# Run tests
bun run test
```
```

</details>
