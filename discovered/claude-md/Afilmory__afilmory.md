---
name: Afilmory__afilmory
source: https://github.com/Afilmory/afilmory/blob/6ab265a8cb1c25e30b8833e0264ac8da859d098a/CLAUDE.md
repo: Afilmory/afilmory
kind: claude-md
stars: 2523
last_pushed: 2026-06-11T12:51:06Z
license: other
score: 10
domains: [monorepo, fullstack-architecture, web-frontend]
tags: [hierarchical-agents, architecture-diagrams, design-system, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# Afilmory/afilmory — claude-md

**Why it's worth keeping:** The nested `AGENTS.md` strategy allows for context-specific depth; the 'Key implications when changing things' section prevents high-level architectural errors; and the ASCII diagram is a perfect tool for mapping complex data flows for an LLM.

**Summary:** A highly sophisticated guide that uses a hierarchical 'Agent' system and ASCII architecture diagrams to explain complex data-injection flows in a monorepo. It provides critical context on how different layers (Builder, SPA, SSR, Backend) interact.

**Source credibility:** High (2,500+ stars on GitHub, active development).

**Recency:** Very current (uses React 19, Next.js 15, and pnpm 10).

**Source:** [Afilmory/afilmory/CLAUDE.md](https://github.com/Afilmory/afilmory/blob/6ab265a8cb1c25e30b8833e0264ac8da859d098a/CLAUDE.md) · 2523★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Authoritative Guides

This repo already has detailed `AGENTS.md` files. Read the one closest to the code you are touching before making non-trivial changes:

- `AGENTS.md` (root) — full commands list, monorepo architecture, manifest/data flow, i18n rules.
- `apps/web/AGENTS.md` — Glassmorphic Depth design system used by the SPA (color/opacity rules, blur, shadows, hover via `data-highlighted`).
- `be/AGENTS.md` — Hono-based "NestJS-style" framework: modules, controllers, providers, decorators, DI via `tsyringe`, request-scoped context via `AsyncLocalStorage`.
- `be/apps/core/AGENTS.md` — backend core service architecture.
- `DEVELOPMENT.md` — self-host quick start and config field reference (`builder.config.ts`, `config.json`).
- `.cursor/rules/*.mdc` — code quality, color (Apple UIKit Tailwind classes), i18n, project description.

When those files contradict anything below, prefer them.

## Commands

```bash
# Dev
pnpm dev                          # SSR wrapper (also serves SPA in dev)
pnpm --filter web dev             # SPA only
pnpm --filter @afilmory/ssr dev
```

</details>
