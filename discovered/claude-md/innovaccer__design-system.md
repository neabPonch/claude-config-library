---
name: innovaccer__design-system
source: https://github.com/innovaccer/design-system/blob/d7e488d1fda182d8febd997685291c66c415534f/CLAUDE.md
repo: innovaccer/design-system
kind: claude-md
stars: 98
last_pushed: 2026-05-19T11:41:56Z
license: mit
score: 9
domains: [web-frontend, design-systems]
tags: [react, typescript, component-library, accessibility]
curated: 2026-06-15
curated_by: config-scout
---

# innovaccer/design-system — claude-md

**Why it's worth keeping:** It includes highly transferable component structure templates and enforces strict quality gates for accessibility and design token adherence which prevents style drift.

**Summary:** This config provides strict architectural, styling, and testing standards for a React design system. It ensures high consistency through explicit component scaffolding rules and mandatory token usage.

**Source credibility:** High; it is a well-structured, real-world open-source design system with recent updates.

**Recency:** Current; utilizes modern Node.js versions and contemporary development workflows.

**Source:** [innovaccer/design-system/CLAUDE.md](https://github.com/innovaccer/design-system/blob/d7e488d1fda182d8febd997685291c66c415534f/CLAUDE.md) · 98★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## What This Repo Is

**Masala Design System (MDS)** — an open-source React + TypeScript component library published as `@innovaccer/design-system`. Components are consumed via named imports; styles ship as a separate CSS bundle (`@innovaccer/design-system/css`).

---

## Environment & Tooling

- **Node ≥ 20.15.0**, **npm ≥ 10.7.0**
- Use `npm` with the committed `package-lock.json`; do not use yarn or pnpm.

---

## Key Commands

| Task | Command |
|---|---|
| Run all tests with coverage | `npm test` |
| Run only changed tests (CI) | `npm run test:ci` |
| Run a single test file | `npx jest path/to/Component.test.tsx` |
| Run a single test by name | `npx jest -t "test name"` |
| Lint TypeScript/JSX | `npm run lint:check` |
| Auto-fix lint issues | `npm run lint` |
| Check CSS formatting | `npm run prettier:check` |
| Auto-fix CSS formatting | `npm run prettier` |
| Type-check | `npm run lint:types` |
| Start Storybook dev server | `npm run dev` (port 5000, also builds CSS watch) |
| Build CSS only | `npm run build-css` |
| Full production build | `npm run build`
```

</details>
