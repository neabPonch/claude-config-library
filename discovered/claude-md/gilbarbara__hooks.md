---
name: gilbarbara__hooks
source: https://github.com/gilbarbara/hooks/blob/41c65e0d90c8c710b349bd5e5619208dfc2dbaac/CLAUDE.md
repo: gilbarbara/hooks
kind: claude-md
stars: 10
last_pushed: 2026-02-07T01:33:29Z
license: mit
score: 9
domains: [web-frontend, react, typescript]
tags: [hooks, ssr, testing-patterns, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# gilbarbara/hooks — claude-md

**Why it's worth keeping:** Excellent use of 'guardrails' like SSR safety patterns, error handling via status objects instead of throws, and specific memoization guidelines. It provides actionable rules for naming conventions and export patterns that prevent architectural drift.

**Summary:** A highly structured guide for a React hooks library that covers build commands, architectural organization, and strict coding standards.

**Source credibility:** High; comes from a specialized-purpose library with clear development standards.

**Recency:** Current; uses modern toolchains like Vitest and tsup.

**Source:** [gilbarbara/hooks/CLAUDE.md](https://github.com/gilbarbara/hooks/blob/41c65e0d90c8c710b349bd5e5619208dfc2dbaac/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a TypeScript React hooks library (@gilbarbara/hooks) that provides a collection of reusable React hooks for state management, side effects, and UI interactions.

## Development Commands

### Build & Development
- `npm run build` - Clean and build the library using tsup (outputs to dist/)
- `npm run watch` - Build and watch for changes
- `npm run clean` - Clean the dist directory

### Testing
- `npm test` - Run tests once
- `npm run test:watch` - Run tests in watch mode
- `npm run test:coverage` - Run tests with coverage
- `vitest run path/to/test.spec.ts` - Run a specific test file
- `vitest watch path/to/test.spec.ts` - Watch a specific test file

### Code Quality
- `npm run lint` - Lint and fix code with ESLint
- `npm run typecheck` - Type check using TypeScript compiler
- `npm run format` - Format code with Prettier
- `npm run validate` - Run full validation (lint, test, build, size check, type validation)

### Bundle Size
- `npm run size` - Check bundle size limits (6kb for ESM and CommonJS)

## Architecture & Structure

### Hook Orga
```

</details>
