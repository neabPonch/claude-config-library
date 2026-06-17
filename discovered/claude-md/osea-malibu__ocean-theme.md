---
name: osea-malibu__ocean-theme
source: https://github.com/osea-malibu/ocean-theme/blob/8b0a62287972c0210f54b278a1b4b5fcfebf7d9d/CLAUDE.md
repo: osea-malibu/ocean-theme
kind: claude-md
stars: 0
last_pushed: 2026-06-15T16:08:55Z
license: other
score: 9
domains: [e-commerce, web-frontend, shopify]
tags: [shopify, liquid, tailwind, vite, web-components]
curated: 2026-06-15
curated_by: config-scout
---

# osea-malibu/ocean-theme — claude-md

**Why it's worth keeping:** Includes highly specific domain 'gotchas' like Liquid metafield nuances and explicit instructions to reuse existing Web Components. It also provides high-level agentic guidance by instructing the model on how to use MCP tools for documentation.

**Summary:** A comprehensive guide for a custom Shopify theme using Vite, Tailwind 4, and Web Components. It defines clear deployment workflows, build pipelines, and strict architectural constraints.

**Source credibility:** High; includes real developer contact info and a structured professional workflow.

**Recency:** Very current; specifically mentions Tailwind 4 and modern AI tool integration patterns (MCP).

**Source:** [osea-malibu/ocean-theme/CLAUDE.md](https://github.com/osea-malibu/ocean-theme/blob/8b0a62287972c0210f54b278a1b4b5fcfebf7d9d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — OSEA Ocean Theme

## Project Overview

Custom Shopify theme for OSEA Malibu, built on Dawn (Online Store 2.0). Powers the DTC storefront at oseamalibu.com. The theme is connected to GitHub — `main` auto-deploys to production.

**Team:** Erin Wilder (erin.wilder@oseamalibu.com) and Jun Kuan (jun.kuan@oseamalibu.com / @junkuan-oseamalibu).

---

## Branch & Deployment Model

| Branch | Purpose |
|---|---|
| `main` | Production — auto-deploys via GitHub Shopify connection |
| `main2`, `main3` | Kept in sync with main; used by marketing team for promotion previews |
| Feature branches | Local dev + Shopify preview themes; deleted after merging |

**Workflow:** Work on feature branches. Preview locally with `shopify theme dev`. If storefront preview is needed, push the branch as a separate Shopify theme, review, then delete after merge.

---

## Commands

```bash
npm run build          # Build JS bundles + Tailwind CSS (one-shot)
npm run dev            # Build in watch mode (incremental, for local development)
npm run format         # Format all files with Prettier
npm run format:check   # Check formatting without writing

shopify theme dev      # Local dev server with liv
```

</details>
