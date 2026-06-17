---
name: rybbit-io__rybbit__claude
source: https://github.com/rybbit-io/rybbit/blob/35f6e768d70f2263d935568b545109f8458b5fef/client/CLAUDE.md
repo: rybbit-io/rybbit
kind: claude-md
stars: 12292
last_pushed: 2026-06-12T21:48:15Z
license: agpl-3.0
score: 9
domains: [web-frontend, nextjs]
tags: [react, typescript, tanstack-query, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# rybbit-io/rybbit — claude-md

**Why it's worth keeping:** It defines an explicit 'API Layer Pattern' with code examples to ensure all data fetching follows a consistent endpoint-to-hook transformation.

**Summary:** A detailed architectural blueprint for a Next.js client covering the stack, project structure, and state management.

**Source credibility:** High; highly starred repository (12k+) with recent maintenance.

**Recency:** Extremely current, utilizing modern technologies like React 19 and Tailwind v4.

**Source:** [rybbit-io/rybbit/client/CLAUDE.md](https://github.com/rybbit-io/rybbit/blob/35f6e768d70f2263d935568b545109f8458b5fef/client/CLAUDE.md) · 12292★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md – Rybbit Client

This file provides guidance to Claude Code when working in the `/client` directory.

## Commands

- `npm run dev` – Start dev server (Next.js + Turbopack, port 3002)
- `npm run build` – Production build
- `npm run lint` – ESLint
- `npm run format` – Prettier format
- `tsc --noEmit` – Type-check without emitting

## Stack

- **Framework**: Next.js 16 (App Router), React 19
- **Styling**: Tailwind CSS v4, Shadcn UI (New York style), Lucide icons
- **State**: Zustand 5 (app/user stores), Jotai (atomic state)
- **Server state**: TanStack React Query 5
- **Auth**: Better-auth (admin, organization, emailOTP, apiKey plugins)
- **Forms**: React Hook Form + Zod
- **i18n**: next-intl (10 locales: en, de, fr, zh, es, pl, it, ko, pt, ja)
- **Charts**: Nivo (bar, calendar, line), D3, Mapbox GL
- **Date/time**: Luxon, date-fns
- **URL state**: nuqs (query string), vaul (drawer)
- **HTTP**: Axios via `authedFetch<T>()` wrapper

## Project Structure

```
src/
├── api/                    # API layer
│   ├── analytics/          # Analytics endpoints + React Query hooks
│   ├── admin/              # Admin endpoints + hooks
│   ├── gsc/                # Google Search Conso
```

</details>
