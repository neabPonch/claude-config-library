---
name: jqlang__playground
source: https://github.com/jqlang/playground/blob/a3b8990c54f212a58db2f35f0c9ec413b14014a3/CLAUDE.md
repo: jqlang/playground
kind: claude-md
stars: 839
last_pushed: 2026-06-01T23:47:18Z
license: mit
score: 9
domains: [web-frontend, nextjs, wasm]
tags: [architecture, data-flow, component-hierarchy]
curated: 2026-06-15
curated_by: config-scout
---

# jqlang/playground — claude-md

**Why it's worth keeping:** The 'Core Data Flow' section is exceptional for helping an agent understand side effects, while the 'Key Patterns' prevent common performance mistakes like blocking the UI thread.

**Summary:** Provides a high-density architectural map including data flow, component hierarchy, and specific execution patterns.

**Source credibility:** High; comes from the official jq playground repository with active maintenance and high star count.

**Recency:** Very current; uses modern tech like Next.js 15.

**Source:** [jqlang/playground/CLAUDE.md](https://github.com/jqlang/playground/blob/a3b8990c54f212a58db2f35f0c9ec413b14014a3/CLAUDE.md) · 839★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A jq playground web application built with Next.js. Users can test jq queries against JSON directly in the browser. All jq processing happens locally via WebAssembly (jq-wasm) - data is only sent to the server when users explicitly share snippets.

Live at: https://play.jqlang.org

## Commands

```bash
# Development (starts Next.js + PostgreSQL via Docker)
docker compose up

# Production build
npm run build
npm run start

# Linting
npm run lint

# Database migrations
npm run prisma:migrate
```

## Architecture

### Core Data Flow

1. **Local Query Execution**: User input → Web Worker (via Comlink) → jq-wasm → Result displayed
2. **Sharing**: User clicks Share → POST /api/snippets → PostgreSQL → Returns shareable URL `/s/[slug]`
3. **Loading Shared**: Visit `/s/[slug]` → Server fetches from DB → Pre-populates Playground state

### Key Components

- **`src/components/Playground.tsx`**: Main orchestrator, manages all state (query, json, http, options, result)
- **`src/workers/`**: Web Worker implementation using Comlink for background jq execution
```

</details>
