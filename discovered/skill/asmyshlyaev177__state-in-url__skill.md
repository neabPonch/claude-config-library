---
name: asmyshlyaev177__state-in-url__skill
source: https://github.com/asmyshlyaev177/state-in-url/blob/1e47260e70f802abacab5993b60b41a25767d426/skills/nextjs-ssr/SKILL.md
repo: asmyshlyaev177/state-in-url
kind: skill
stars: 416
last_pushed: 2026-06-15T18:55:32Z
license: mit
score: 9
domains: [web-frontend, nextjs, react]
tags: [ssr, hydration, url-state, server-components]
curated: 2026-06-15
curated_by: config-scout
---

# asmyshlyaev177/state-in-url — skill

**Why it's worth keeping:** It includes a highly specific 'Proxy + header' pattern to solve the missing searchParams issue in server layouts and explicitly addresses breaking changes in Next.js 15 (Promise-based searchParams).

**Summary:** Provides specific architectural patterns for managing URL state in Next.js App Router to prevent hydration mismatches and SSR sync issues.

**Source credibility:** High; the source is an active, starred library specifically addressing deep framework integration edge cases.

**Recency:** Highly current, accounting for Next.js 15+ async searchParams changes.

**Source:** [asmyshlyaev177/state-in-url/skills/nextjs-ssr/SKILL.md](https://github.com/asmyshlyaev177/state-in-url/blob/1e47260e70f802abacab5993b60b41a25767d426/skills/nextjs-ssr/SKILL.md) · 416★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nextjs-ssr
description: >
  SSR-safe useUrlState in Next.js App Router. Forward searchParams from server
  pages (awaiting the Promise in Next.js 15+), call useSearchParams() in pure
  client components, decide between useHistory true/false, and use a Proxy
  (formerly middleware) to expose query params to server layouts. App Router
  only — Pages Router is not supported. Load this skill for any use of
  state-in-url/next or anytime URL state must be correct on first paint.
type: framework
library: state-in-url
framework: react
library_version: '6.1.3'
requires:
  - feature-state-hook
sources:
  - 'asmyshlyaev177/state-in-url:packages/urlstate/next/useUrlState/useUrlState.ts'
  - 'asmyshlyaev177/state-in-url:packages/example-nextjs16/src/middleware.ts'
  - 'asmyshlyaev177/state-in-url:README.md#with-server-side-rendering'
---

This skill builds on `state-in-url/feature-state-hook`. Read it first for the module-scoped default-state rule.

# state-in-url — Next.js App Router SSR

Without `searchParams`, the first render of a `useUrlState` component has no URL knowledge. It renders defaults, then a client `useEffect` re-syncs from the URL → visible flash and a React hydratio
```

</details>
