---
name: kazupon__gunshi
source: https://github.com/kazupon/gunshi/blob/1af9300fc483d8e7347bdceb57382ee40736da4f/CLAUDE.md
repo: kazupon/gunshi
kind: claude-md
stars: 423
last_pushed: 2026-06-15T06:33:25Z
license: mit
score: 9
domains: [cli-tools, javascript, monorepo]
tags: [typescript, pnpm, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# kazupon/gunshi — claude-md

**Why it's worth keeping:** The explicit mapping of the monorepo structure and detailed command list allows Claude to navigate packages and run tasks without manual exploration; includes architectural patterns to guide implementation.

**Summary:** Provides deep structural visibility of a complex monorepo, including package relationships and specific development workflows.

**Source credibility:** Highly credible source with significant GitHub stars and extremely active maintenance.

**Recency:** Very current, utilizing modern tooling like pnpm, Vitest, and JSR.

**Source:** [kazupon/gunshi/CLAUDE.md](https://github.com/kazupon/gunshi/blob/1af9300fc483d8e7347bdceb57382ee40736da4f/CLAUDE.md) · 423★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Gunshi is a modern JavaScript command-line library for creating CLI applications. It supports multiple JavaScript runtimes (Node.js, Deno, Bun) and provides features like declarative command configuration, type safety, composable sub-commands, lazy loading, internationalization, and a powerful plugin system.

This is a **pnpm workspace monorepo** containing the core library, plugins, utilities, and documentation. The project emphasizes type safety, runtime compatibility, minimal dependencies, and extensibility through a well-designed plugin architecture.

## Essential Commands

```sh
# Install dependencies
pnpm install

# Build all packages
pnpm build

# Run all tests with type checking
pnpm test

# Run E2E tests
pnpm e2e

# Run tests for specific packages
pnpm test:core                  # Core gunshi package
pnpm test:plugin-global         # Global options plugin
pnpm test:plugin-i18n           # i18n plugin
pnpm test:plugin-renderer       # Renderer plugin
pnpm test:plugin-completion     # Completion plugin

# Run linter (ESLint, Prettier, Knip
```

</details>
