---
name: happo__happo
source: https://github.com/happo/happo/blob/f4c28a7dfaa212f7036840d8d2993ce3301996d1/CLAUDE.md
repo: happo/happo
kind: claude-md
stars: 511
last_pushed: 2026-06-12T22:48:23Z
license: unknown
score: 9
domains: [cli-tools, testing-infrastructure]
tags: [architecture, build-system, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# happo/happo — claude-md

**Why it's worth keeping:** The 'Package Outputs' mapping and the high-level 'Key Data Flow' section are exceptional for preventing hallucinations during build/debug tasks.

**Summary:** Detailed documentation of build processes, directory purposes, and complex cross-package data flows.

**Source credibility:** High; a popular open-source tool (511 stars) with very recent activity.

**Recency:** Current; uses modern tooling like pnpm, esbuild, and Node's native test runner.

**Source:** [happo/happo/CLAUDE.md](https://github.com/happo/happo/blob/f4c28a7dfaa212f7036840d8d2993ce3301996d1/CLAUDE.md) · 511★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Happo is an open source library for integrating with [happo.io](https://happo.io) — a visual and accessibility regression testing platform. It ships as a Node.js package with a CLI tool (`happo`) and integration adapters for Storybook, Cypress, Playwright, and custom setups.

## Commands

```bash
pnpm install        # Install dependencies
pnpm build          # Full build: type-check + esbuild dist
pnpm build:types    # TypeScript declarations build (tsc project refs; emits to dist/ and tmp/tsc/)
pnpm build:dist     # esbuild bundling only
pnpm lint           # ESLint
pnpm test           # Run unit tests (Node test runner)
pnpm all            # Run everything in parallel: lint, build:types, test, test:playwright
pnpm clean          # Remove dist/, tmp/tsc, tmp/happo-custom
```

### Running a single test or subset of tests

The test script (`scripts/test.ts`) wraps Node's built-in test runner with `fzf`-based file selection:

```bash
# Run tests matching a file pattern (uses fzf fuzzy matching)
pnpm test loadConfig

# Run tests matching a test name pattern
```

</details>
