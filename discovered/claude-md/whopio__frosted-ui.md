---
name: whopio__frosted-ui
source: https://github.com/whopio/frosted-ui/blob/a6cdb68f06c6fed711fcb3fde1cd9d7d02ae47a2/CLAUDE.md
repo: whopio/frosted-ui
kind: claude-md
stars: 255
last_pushed: 2026-06-05T16:09:52Z
license: other
score: 7
domains: [web-frontend, design-system]
tags: [monorepo, pnpm, react, tailwindcss]
curated: 2026-06-14
curated_by: config-scout
---

# whopio/frosted-ui — claude-md

**Why it's worth keeping:** The distinction between generic app commands and package-specific filter patterns is crucial for navigating workspaces. It also explicitly mentions modern tools like Tailwind v4.

**Summary:** Provides essential command filtering for a pnpm monorepo structure and defines specific styling standards.

**Source credibility:** High; part of an official design system from Whop.

**Recency:** Very current; uses modern pnpm workspace patterns and latest CSS frameworks.

**Source:** [whopio/frosted-ui/CLAUDE.md](https://github.com/whopio/frosted-ui/blob/a6cdb68f06c6fed711fcb3fde1cd9d7d02ae47a2/CLAUDE.md) · 255★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build/Test/Lint Commands

### Monorepo
- **Dev server**: `pnpm dev --filter=<app>` (Example: `pnpm dev --filter=tailwind`)
- **Build**: `pnpm build --filter=<app>`
- **Lint**: `pnpm lint --filter=<app>`
- **TypeCheck**: `pnpm typecheck --filter=<app>`

### Frosted UI Package
- **Dev server**: `pnpm --filter="frosted-ui" dev`
- **Build**: `pnpm --filter="frosted-ui" build`
- **Lint**: `pnpm --filter="frosted-ui" lint`
- **Storybook**: `pnpm --filter="frosted-ui" storybook`

## Code Style Guidelines

- **TypeScript**: Strict typing, ES2020 modules, 120 char line width, 2-space indentation
- **React**: Functional components with hooks, JSX format
- **CSS**: Tailwind CSS v4, PostCSS with nesting/custom media/imports
- **Formatting**: Single quotes, semicolons required, trailing commas in multiline
- **Project**: pnpm workspaces with Turborepo, NextJS for applications
- **Commits**: Semantic commit messages (feat, fix, docs, style, refactor, perf, test, chore)
- **Quality**: ESLint for linting, Prettier for formatting, Storybook for component docs
```

</details>
