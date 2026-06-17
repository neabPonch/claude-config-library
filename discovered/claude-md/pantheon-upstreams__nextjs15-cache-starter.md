---
name: pantheon-upstreams__nextjs15-cache-starter
source: https://github.com/pantheon-upstreams/nextjs15-cache-starter/blob/9d51900f5a7808eb62bb41e561db24a23ae0bd5f/claude.md
repo: pantheon-upstreams/nextjs15-cache-starter
kind: claude-md
stars: 0
last_pushed: 2026-04-13T20:51:11Z
license: unknown
score: 8
domains: [web-frontend, caching]
tags: [nextjs, architecture, cache-management]
curated: 2026-06-16
curated_by: config-scout
---

# pantheon-upstreams/nextjs15-cache-starter — claude-md

**Why it's worth keeping:** It includes critical technical 'gotchas' (middleware incompatibility) and explains the reasoning behind specific configuration choices to prevent an AI from reversing intentional optimizations.

**Summary:** Provides high-context architectural documentation for a Next.js 15 project focused on custom cache management and API routing.

**Source credibility:** High; likely authored by infrastructure engineers at Pantheon given the organization name.

**Recency:** Highly current, explicitly targeting Next.js 15 and Tailwind v4.

**Source:** [pantheon-upstreams/nextjs15-cache-starter/claude.md](https://github.com/pantheon-upstreams/nextjs15-cache-starter/blob/9d51900f5a7808eb62bb41e561db24a23ae0bd5f/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev          # Start development server
npm run build        # Production build
npm run start        # Start production server
npm run lint         # Run ESLint
```

## Architecture

This is a **Next.js 15** app (App Router) that demonstrates custom cache handlers via the `@pantheon-systems/nextjs-cache-handler` package. It uses Tailwind CSS v4 for styling.

### Cache System

The cache handler is configured in `cache-handler.mjs` and wired into Next.js via `next.config.mjs` (`cacheHandler` + `cacheMaxMemorySize: 0` to disable in-memory caching). The handler auto-selects between GCS and file-based storage (GCS is automatically configured when deployed on Pantheon).

Cache stats and clearing are exposed via `@pantheon-systems/nextjs-cache-handler`'s `getSharedCacheStats` and `clearSharedCache` exports, used in `app/api/cache-stats/route.ts`.

### Surrogate Keys

`next.config.mjs` sets `Surrogate-Key` headers on responses for CDN cache invalidation. Routes under `/blogs` get structured keys (e.g., `blog-:slug`, `blog-index-tag-:tag`); other
```

</details>
