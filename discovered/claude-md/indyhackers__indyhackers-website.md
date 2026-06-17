---
name: indyhackers__indyhackers-website
source: https://github.com/indyhackers/indyhackers-website/blob/5f217ad3fc243b13d482a33658d2a021aeff032d/CLAUDE.md
repo: indyhackers/indyhackers-website
kind: claude-md
stars: 3
last_pushed: 2026-06-15T03:39:20Z
license: unknown
score: 8
domains: [web-frontend, fullstack]
tags: [vue3, pocketbase, msw, vitest]
curated: 2026-06-15
curated_by: config-scout
---

# indyhackers/indyhackers-website — claude-md

**Why it's worth keeping:** The explanation of the MSW mock data synchronization process is highly specific and prevents agent confusion. The inclusion of exact single-file test commands optimizes Claude's tool use efficiency.

**Summary:** Provides essential context for a unique dual-mode development workflow using MSW mocking and PocketBase. It includes high-value specific commands for granular test execution.

**Source credibility:** Low star count, but the file demonstrates high technical maturity and professional documentation standards.

**Recency:** Very current; utilizes modern Vue 3/Vite and PocketBase patterns.

**Source:** [indyhackers/indyhackers-website/CLAUDE.md](https://github.com/indyhackers/indyhackers-website/blob/5f217ad3fc243b13d482a33658d2a021aeff032d/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

IndyHackers Redux — a Vue 3 + PocketBase community site for Indianapolis tech. Frontend built with Vite, Bootstrap 5 / Bootstrap-Vue-Next, and Pinia. Backend is PocketBase (Go-based BaaS with SQLite). JavaScript only (no TypeScript).

## Commands

```bash
npm run dev          # Vite dev server (localhost:5173)
npm run build        # Production build
npm run lint         # ESLint with auto-fix
npm run format       # Prettier formatting
npm run test:unit    # Vitest unit tests (interactive watch mode)
npm run test:e2e     # Playwright e2e tests (install browsers first: npx playwright install)
```

Run a single unit test file: `npx vitest run src/components/__tests__/SomeTest.spec.js`
Run a single e2e test: `npm run test:e2e -- --project=chromium e2e/some.spec.js`

Docker/Task commands for local PocketBase development:
```bash
task run-dev         # Run PocketBase + Vue with hot reload via docker-compose
task build-dev       # Build dev Docker image
```

## Architecture

### Dual-Mode Development (MSW Mocking)

The app runs in two modes:
- **Develop
```

</details>
