---
name: sorge13248__lightschool
source: https://github.com/sorge13248/lightschool/blob/63180d7979a7c73bb4d496af2b15b25ae05ec202/CLAUDE.md
repo: sorge13248/lightschool
kind: claude-md
stars: 0
last_pushed: 2026-04-17T19:29:56Z
license: agpl-3.0
score: 9
domains: [web-frontend, backend-api, security]
tags: [laravel, inertia, svelte, encryption]
curated: 2026-06-16
curated_by: config-scout
---

# sorge13248/lightschool — claude-md

**Why it's worth keeping:** It documents non-obvious logic like the hybrid encryption layers and specific controller dispatch patterns, which prevents the AI from introducing security flaws or architectural drift.

**Summary:** Provides an exhaustive technical breakdown of a Laravel/Inertia/Svelte application, covering request flows, frontend organization, and security architecture.

**Source credibility:** The repository has low visibility, but the file is clearly hand-crafted by a developer with high standards for documentation.

**Recency:** Highly current; uses modern tooling like Vite and Svelte.

**Source:** [sorge13248/lightschool/CLAUDE.md](https://github.com/sorge13248/lightschool/blob/63180d7979a7c73bb4d496af2b15b25ae05ec202/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Development server (Docker)
docker compose up

# Run tests (clears config cache first)
npm test                          # alias for: artisan config:clear && artisan test

# Run a single test file
php artisan test tests/Feature/AuthTest.php

# Run a single test by name
php artisan test --filter "test name"

# CSS/JS build
npm run dev     # Vite dev server
npm run build   # Production build

# Database
php artisan migrate --force --seed

# Laravel utilities
php artisan view:clear
php artisan config:clear
```

## Architecture

### Request Flow

There are two classes of requests:

**Page requests** go through Laravel routes → `PageController` → `Inertia::render('path/Page', [props])`. Inertia serialises the props as JSON and the single root Blade view (`resources/views/app.blade.php`) boots the Svelte app. The browser receives a fully hydrated Svelte component.

**API requests** go through Laravel routes → a feature controller's `handle(Request $request)` method → a `match($request->query('type'))` dispatcher → specific sub-operation. The response
```

</details>
