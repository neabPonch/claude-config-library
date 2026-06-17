---
name: p-m-p__slider
source: https://github.com/p-m-p/slider/blob/77c3adc00238d2a68fbd039899533def43f8a360/CLAUDE.md
repo: p-m-p/slider
kind: claude-md
stars: 889
last_pushed: 2026-05-15T05:42:43Z
license: mit
score: 8
domains: [web-frontend, monorepo, typescript]
tags: [monorepo, pnpm, architecture-guide, component-library]
curated: 2026-06-15
curated_by: config-scout
---

# p-m-p/slider — claude-md

**Why it's worth keeping:** Provides specific pnpm workspace/filtering commands which are crucial for monorepos, and maps the logic flow (state-store to transition-queue) to help Claude understand intent before reading code.

**Summary:** A detailed guide for a TypeScript monorepo that outlines package structures, command patterns, and architectural components.

**Source credibility:** High; popular library (889 stars) with recent maintenance.

**Recency:** Very current; uses modern tooling like pnpm, Vitest, and esbuild.

**Source:** [p-m-p/slider/CLAUDE.md](https://github.com/p-m-p/slider/blob/77c3adc00238d2a68fbd039899533def43f8a360/CLAUDE.md) · 889★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project structure

BoxSlider is a monorepo containing a modern content slider library with multiple distribution formats:

- `packages/slider/` - Core TypeScript slider library with zero dependencies
- `packages/react/` - React component wrappers
- `packages/components/` - Web Components implementation
- `packages/docs/` - Docusaurus documentation site

The library provides multiple slide transition effects (carousel, fade, cube, tile) and can be used standalone or via React/Web Components.

## Commands

**Build & Development:**

- `pnpm build` - Build all packages
- `pnpm dev` - Start examples development server
- `pnpm clean` - Clean all build artifacts

**Testing:**

- `pnpm test` - Run all tests with Vitest
- `pnpm test:coverage` - Run tests with coverage report
- `pnpm test:ui` - Open Vitest UI

**Storybook:**

- `pnpm storybook` - Start Storybook development server
- `pnpm build-storybook` - Build Storybook for production

**Code Quality:**

- `pnpm lint` - Run Prettier check and ESLint
- `pnpm format` - Format code with Prettier

**Package Management:**

-
```

</details>
