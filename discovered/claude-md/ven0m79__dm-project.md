---
name: ven0m79__dm-project
source: https://github.com/ven0m79/dm-project/blob/26cd7b7a4f793c463ebd3c06c4dd0463f110afc2/Claude.md
repo: ven0m79/dm-project
kind: claude-md
stars: 0
last_pushed: 2026-05-06T19:01:15Z
license: unknown
score: 8
domains: [web-frontend, e-commerce, nextjs]
tags: [nextjs, tailwindcss, woocommerce, i18n]
curated: 2026-06-14
curated_by: config-scout
---

# ven0m79/dm-project — claude-md

**Why it's worth keeping:** It documents high-level business logic like breadcrumb exclusion rules and specific server-side caching behaviors which are critical for an AI to know before refactoring.

**Summary:** A highly detailed architectural guide for a Next.js/WooCommerce e-commerce application with complex i18n routing.

**Source credibility:** Low social proof (0 stars), but demonstrates expert knowledge of modern stack versions (React 19, Tailwind 4).

**Recency:** Extremely current; uses bleeding-edge dependencies.

**Source:** [ven0m79/dm-project/Claude.md](https://github.com/ven0m79/dm-project/blob/26cd7b7a4f793c463ebd3c06c4dd0463f110afc2/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev        # Start development server
npm run build      # Production build
npm run start      # Start production server
npm run lint       # Run ESLint
```

No test suite is configured.

## Architecture

**Stack:** Next.js 16 (App Router) + React 19 + TypeScript + Tailwind CSS 4 + WooCommerce headless

### Routing

All user-facing pages live under [app/\[locale\]/](app/[locale]/) for i18n. Supported locales are `ua` (default) and `en`, handled by **next-intl** with `prefix: "as-needed"` — Ukrainian URLs have no prefix, English gets `/en/`. Locale detection is disabled; the default is always `ua`.

The i18n configuration lives in [i18n/routing.ts](i18n/routing.ts) (locale definitions), [i18n/request.ts](i18n/request.ts) (server config), and [i18n/navigation.ts](i18n/navigation.ts) (typed `Link`, `redirect`, etc.).

[proxy.ts](proxy.ts) is the actual middleware file (re-exported via `middleware.ts`). It handles:
- `www.` → canonical redirects (301)
- Legacy `/shares/*` URLs → new catalog product URLs or WordPress `/info/*` pages
- `/home`
```

</details>
