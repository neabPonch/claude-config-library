---
name: rjsf-team__react-jsonschema-form
source: https://github.com/rjsf-team/react-jsonschema-form/blob/cb432190cce9285194f37ec3e3b0f0fbff3c3d88/CLAUDE.md
repo: rjsf-team/react-jsonschema-form
kind: claude-md
stars: 15804
last_pushed: 2026-06-13T17:19:56Z
license: apache-2.0
score: 9
domains: [web-frontend, monorepo]
tags: [architecture-patterns, npm-workspaces, react]
curated: 2026-06-15
curated_by: config-scout
---

# rjsf-team/react-jsonschema-form — claude-md

**Why it's worth keeping:** It explains high-level mental models like the 'Registry pattern' and component hierarchies, allowing Claude to understand system-wide logic instead of just file locations.

**Summary:** Provides a deep architectural breakdown of the monorepo, including specific command patterns for individual packages and shared test suites.

**Source credibility:** High; from a popular, actively maintained React library with 15k+ stars.

**Recency:** Very current; utilizes modern tooling like Nx, Vitest, and Node 20.

**Source:** [rjsf-team/react-jsonschema-form/CLAUDE.md](https://github.com/rjsf-team/react-jsonschema-form/blob/cb432190cce9285194f37ec3e3b0f0fbff3c3d88/CLAUDE.md) · 15804★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Install dependencies
npm install

# Build all packages (parallel)
npm run build

# Build all packages (sequential, use if parallel causes issues)
npm run build-serial

# Run all tests
npm test

# Lint
npm run lint

# Prettier check / format
npm run cs-check
npm run cs-format

# Run a single package's tests
cd packages/core && npm test

# Watch mode for a single package
cd packages/core && npm run test:watch

# Update snapshots
cd packages/snapshot-tests && npm run test:update

# Start the playground (interactive demo)
cd packages/playground && npm start

# Full sanity check (lint + build + test)
npm run sanity-check
```

Individual package builds output three module formats: `build:cjs`, `build:esm`, `build:umd`.

## Architecture

This is an **npm workspaces + Nx** monorepo. All packages live under `packages/` and are scoped as `@rjsf/*`.

### Package roles

| Package | Role |
|---|---|
| `@rjsf/utils` | Shared types, 80+ utility functions, schema helpers. No UI dependencies. |
| `@rjsf/core` | Core `Form` component, Bootstrap 3 as default them
```

</details>
