---
name: rogerleecormier__spearyx
source: https://github.com/rogerleecormier/spearyx/blob/41dadea12053ea7385b9b9fd96c724944d1e0192/claude.md
repo: rogerleecormier/spearyx
kind: claude-md
stars: 0
last_pushed: 2026-05-07T16:36:41Z
license: unknown
score: 9
domains: [web-frontend, fullstack, design-systems]
tags: [tanstack, tailwind-v4, cloudflare-workers, ui-kit]
curated: 2026-06-15
curated_by: config-scout
---

# rogerleecormier/spearyx — claude-md

**Why it's worth keeping:** It uses 'negative constraints' to prevent common errors (e.g., no dark mode, don't touch tailwind.config) and provides a specific hierarchy for UI component usage.

**Summary:** A high-density configuration for a TanStack Start and Cloudflare stack that enforces strict architectural and styling constraints.

**Source credibility:** Low popularity/stars, but the technical depth suggests high-quality individual authorship.

**Recency:** Very current; includes modern Tailwind v4 CSS-first architecture patterns.

**Source:** [rogerleecormier/spearyx/claude.md](https://github.com/rogerleecormier/spearyx/blob/41dadea12053ea7385b9b9fd96c724944d1e0192/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Custom Instructions for Spearyx

You are an expert software engineer tasked with assisting on the Spearyx monorepo. Before providing code, take a deep breath and "think" about how the request aligns with the following architectural guardrails.

## System Architecture & Stack
- **Framework:** TanStack Start (React SSR) + Vite.
- **Data Fetching:** TanStack Query.
- **Backend:** Cloudflare Workers + Cloudflare D1 (SQLite).
- **ORM:** Drizzle ORM (Workers connect *directly* to D1).
- **Monorepo Tooling:** Turborepo + npm workspaces.

## Tailwind CSS v4 & Styling Rules
- **CRITICAL:** We use Tailwind v4 in a **CSS-first architecture**. 
- Do **NOT** instruct me to modify `tailwind.config.ts` unless it is strictly for a legacy tool compatibility shim.
- All theme extensions go in `packages/shared-config/styles.css` using the `@theme` directive.
- **NO Dark Mode:** Do not generate `dark:` classes. The application is strictly light-mode.
- **Semantic Colors:** Never use hex codes in markup. Use the design system tokens (e.g., `primary-500`, `success-500`, `slate-900`).
- **Typography:** Do not use raw `h1`-`h6` tags for styled text. Always use `@spearyx/ui-kit/Typography` compone
```

</details>
