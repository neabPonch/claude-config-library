---
name: mxluk__shortener
source: https://github.com/mxluk/shortener/blob/7feec12ad626097e8b180af5c96487a5baa1d0ee/claude.md
repo: mxluk/shortener
kind: claude-md
stars: 0
last_pushed: 2025-12-04T17:12:49Z
license: unknown
score: 8
domains: [web-backend, serverless]
tags: [url-shortener, cloudflare-workers]
curated: 2026-06-14
curated_by: config-scout
---

# mxluk/shortener — claude-md

**Why it's worth keeping:** It provides exact implementation details for the custom base-59 hashing and collision handling logic, which is essential for an agent to maintain or refactor core system behaviors without error.

**Summary:** A high-density technical breakdown of a serverless architecture including specific algorithmic logic and development workflows.

**Source credibility:** 0 stars; likely a personal side project with high technical documentation quality.

**Recency:** Highly current (mentions 2025 compatibility dates and pnpm v10).

**Source:** [mxluk/shortener/claude.md](https://github.com/mxluk/shortener/blob/7feec12ad626097e8b180af5c96487a5baa1d0ee/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FUC.MOE URL Shortener

A serverless URL shortening service built on Cloudflare Workers with a static Astro frontend.

## What It Does

This is a URL shortening service that allows users to:
- Generate short URLs from long URLs with auto-generated hashes
- Create custom short URLs with user-defined slugs (e.g., `fuc.moe/go+https://google.com`)
- Redirect short URLs to their original destinations
- Preserve query parameters and URL fragments during shortening

The service uses a deterministic hashing algorithm that generates consistent short codes for the same URL, with collision handling built in.

## Technology Stack

### Backend (Cloudflare Worker)
- **Cloudflare Workers**: Serverless edge computing platform
- **TypeScript**: Strictly typed with ES2021 target
- **Cloudflare KV**: Key-value storage for URL mappings
- **Wrangler**: Cloudflare Workers CLI tool for deployment

### Frontend (Static Site)
- **Astro**: Static site generator (v4.11.5+)
- **TypeScript**: For type safety
- **jQuery**: (v3.7.1) For DOM manipulation and AJAX
- **CSS**: Component-scoped styles with Astro

### Testing
- **Vitest**: Testing framework
- **@cloudflare/vitest-pool-workers**: Cloudflare Workers te
```

</details>
