---
name: apex-dev-tools__test-runner
source: https://github.com/apex-dev-tools/test-runner/blob/f258e42131d0aa16b0a15037f488b62ae6536299/CLAUDE.md
repo: apex-dev-tools/test-runner
kind: claude-md
stars: 3
last_pushed: 2026-06-14T20:22:31Z
license: bsd-3-clause
score: 9
domains: [cli-tools, testing-frameworks, backend-infrastructure]
tags: [architecture-heavy, workflow-driven, test-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# apex-dev-tools/test-runner — claude-md

**Why it's worth keeping:** Uses a 'collaborators' pattern to explain object relationships and documents exact algorithmic steps for core logic like the reliability/rerun flow.

**Summary:** Provides a high-level architectural overview and detailed orchestration flows for a complex test runner library.

**Source credibility:** High; well-maintained project with clear, specialized purpose.

**Recency:** Current; uses modern tooling (pnpm, corepack) and TypeScript standards.

**Source:** [apex-dev-tools/test-runner/CLAUDE.md](https://github.com/apex-dev-tools/test-runner/blob/f258e42131d0aa16b0a15037f488b62ae6536299/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

`@apexdevtools/test-runner` is a **library** (not a CLI) that runs Salesforce Apex unit tests in parallel with reliability features layered on top of `@salesforce/apex-node` and `jsforce`. It is consumed by other tools that pass it a Salesforce `Connection`. Its job is to maximise the chance of a clean test run by detecting and re-running tests that fail for non-genuine reasons (row-lock/deadlock errors), filling in missing results, and restarting runs that hang.

## Commands

This project uses **pnpm** (v8.9.2, via corepack). `.npmrc` pins the registry to npmjs.org to override any user private registry.

```sh
pnpm install
pnpm build                 # tsc -> ./lib
pnpm test                  # jest --coverage --runInBand (single-worker; tests rely on it)
pnpm test:watch            # jest --watch
pnpm lint                  # eslint ./src/ --fix
pnpm clean                 # rm -rf ./lib

# Run a single test file / test
pnpm test -- test/runner/TestRunner.spec.ts
pnpm test -- -t "name of test"

# Verify the webpack bundle (used by consumers); must run w
```

</details>
