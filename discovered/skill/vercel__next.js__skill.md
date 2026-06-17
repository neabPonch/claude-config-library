---
name: vercel__next.js__skill
source: https://github.com/vercel/next.js/blob/901c0803941c6ae39c2670f9ea3c05cf6bc8b8c2/.agents/skills/react-vendoring/SKILL.md
repo: vercel/next.js
kind: skill
stars: 140031
last_pushed: 2026-06-16T06:24:28Z
license: mit
score: 9
domains: [web-framework, build-systems, javascript]
tags: [react, nextjs, bundling, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# vercel/next.js — skill

**Why it's worth keeping:** It provides exact code patterns for polyfilling Node-only APIs and enforces strict architectural rules to prevent runtime production errors that standard linting might miss.

**Summary:** Defines the complex internal vendoring architecture of React within Next.js, specifically for the App Router and server-side boundaries.

**Source credibility:** Extremely high; sourced from the official Next.js repository with massive industry adoption.

**Recency:** Highly current, reflecting modern React Server Component and Turbopack architectures.

**Source:** [vercel/next.js/.agents/skills/react-vendoring/SKILL.md](https://github.com/vercel/next.js/blob/901c0803941c6ae39c2670f9ea3c05cf6bc8b8c2/.agents/skills/react-vendoring/SKILL.md) · 140031★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: react-vendoring
description: >
  React vendoring and react-server layer boundaries. Use when editing
  entry-base.ts, $$compiled.internal.d.ts, compiled/react* packages,
  or taskfile.js copy_vendor_react. Covers the entry-base.ts boundary
  (all react-server-dom-webpack/* imports must go through it), vendored
  React channels, type declarations, Turbopack remap to
  react-server-dom-turbopack, ComponentMod access patterns, and ESLint
  suppression for guarded requires.
metadata:
  internal: true
---

# React Vendoring

Use this skill for changes touching vendored React, `react-server-dom-webpack/*`, or react-server layer boundaries.

## App Router Vendoring

React is NOT resolved from `node_modules` for App Router. It's vendored into `packages/next/src/compiled/` during `pnpm build` (task: `copy_vendor_react()` in `taskfile.js`). Pages Router resolves React from `node_modules` normally.

- **Two channels**: stable (`compiled/react/`) and experimental (`compiled/react-experimental/`). The runtime bundle webpack config aliases to the correct channel via `makeAppAliases({ experimental })`.

## `entry-base.ts` Boundary

Only `entry-base.ts` is compiled in rspack's `(react-se
```

</details>
