---
name: bartstc__vite-ts-react-template
source: https://github.com/bartstc/vite-ts-react-template/blob/a1762e092211eaaada4ad8a986692f521001f795/CLAUDE.md
repo: bartstc/vite-ts-react-template
kind: claude-md
stars: 120
last_pushed: 2026-06-01T06:06:10Z
license: mit
score: 9
domains: [web-frontend, react]
tags: [spec-driven, self-improvement, surgical-changes, agentic-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# bartstc/vite-ts-react-template — claude-md

**Why it's worth keeping:** Includes a 'Self-Improvement Loop' using a lessons file to prevent recurring errors and mandates a 'Plan Mode' for complex tasks to ensure architectural alignment.

**Summary:** An advanced operational manual that enforces surgical code changes and high-level agentic workflows. It includes sophisticated patterns for planning, verification, and automated learning.

**Source credibility:** High; the repository is extremely well-maintained with very recent updates reflecting modern stack versions.

**Recency:** Highly current, utilizing cutting-edge technologies like React 19 and Vite 7.

**Source:** [bartstc/vite-ts-react-template/CLAUDE.md](https://github.com/bartstc/vite-ts-react-template/blob/a1762e092211eaaada4ad8a986692f521001f795/CLAUDE.md) · 120★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project

React SPA built with Vite using feature slice architecture with clean architecture principles.

## Stack

TypeScript SPA. React 19, Vite 7, React Router 7, TanStack Query, Zustand, XState, Chakra UI, i18next. Testing: Vitest, Storybook, Playwright, MSW.

## Commands

- `pnpm dev` — start dev server (port 5173)
- `pnpm dev:all` — start both frontend (port 5173) and local API server (port 3001)
- `pnpm typecheck` — type-check all sources (src, e2e, stories, tests)
- `pnpm lint --fix` — lint and auto-fix
- `pnpm test` — all tests (unit + storybook)
- `pnpm test:e2e` — Playwright E2E (headless)
- `pnpm storybook` — component dev (port 6006)

Package manager: PNPM only. Path alias: `@/*` → `src/`.

## Core Principles

- **Simplicity first** — make every change as simple as possible, minimize code impact, choose the boring solution
- **Surgical changes** — touch only what the task requires; don't refactor, reformat, or "improve" adjacent code. Remove only the orphans your own changes create
- When unsure about requirements or business logic, ask the developer — never assume
- When multiple interpretations exist, present them — don't pick silently
- For changes >300 LOC or >3 f
```

</details>
