---
name: mattpocock__evalite
source: https://github.com/mattpocock/evalite/blob/e18a793789400b9292f92465d1084344340aef9b/CLAUDE.md
repo: mattpocock/evalite
kind: claude-md
stars: 1592
last_pushed: 2026-04-28T18:31:29Z
license: mit
score: 9
domains: [cli-tools, testing-frameworks, monorepo]
tags: [typescript, pnpm-workspace, vitest]
curated: 2026-06-15
curated_by: config-scout
---

# mattpocock/evalite — claude-md

**Why it's worth keeping:** Includes specific 'pnpm --filter' patterns to prevent directory-jumping errors and provides an architectural 'execution flow' that explains how data moves from .eval.ts files into the database.

**Summary:** Provides a highly structured guide for navigating a complex pnpm monorepo and understanding the internal execution flow of evaluation files.

**Source credibility:** High: highly starred (1500+) and actively maintained repository.

**Recency:** Very current; explicitly references Claude Code/claude.ai/code.

**Source:** [mattpocock/evalite/CLAUDE.md](https://github.com/mattpocock/evalite/blob/e18a793789400b9292f92465d1084344340aef9b/CLAUDE.md) · 1592★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Evalite is a TypeScript-native, local-first tool for testing LLM-powered apps built on Vitest. It allows developers to write evaluations (evals) as `.eval.ts` files that run like tests.

## Configuration

The primary configuration method is `evalite.config.ts`. While `vitest.config.ts` is still supported for backward compatibility, it is not documented and `evalite.config.ts` should be used for all configuration needs.

## Development Commands

**Development mode** (recommended for working on Evalite itself):

```bash
pnpm run dev
```

This runs:

- TypeScript type checker on `evalite` package
- Tests in `evalite-tests` package
- Live reload for both packages

**Build all packages**:

```bash
pnpm build
```

This builds `evalite` package first, then `evalite-ui`, copying UI assets to `packages/evalite/dist/ui`.

**Run CI pipeline** (build, test, lint):

```bash
pnpm ci
```

**Test the example evals**:

```bash
pnpm run example
# Or: cd packages/example && pnpm evalite watch
```

**Run single package tests**:

```bash
cd packages/evalite && pnpm test
cd p
```

</details>
