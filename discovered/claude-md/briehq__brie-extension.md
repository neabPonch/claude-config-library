---
name: briehq__brie-extension
source: https://github.com/briehq/brie-extension/blob/b18e550026e4acf322815bd91200692593397d91/CLAUDE.md
repo: briehq/brie-extension
kind: claude-md
stars: 715
last_pushed: 2026-06-15T18:06:21Z
license: apache-2.0
score: 9
domains: [web-frontend, browser-extension, monorepo]
tags: [chrome-extension, pnpm, turborepo, typescript, react]
curated: 2026-06-16
curated_by: config-scout
---

# briehq/brie-extension — claude-md

**Why it's worth keeping:** Uses structured tables to map entry points/packages to their purposes and defines highly specific command patterns and file-naming conventions that prevent AI hallucinations regarding project structure.

**Summary:** Provides deep structural context for a complex browser extension monorepo, mapping entry points, communication patterns, and specific build processes.

**Source credibility:** High; a popular open-source repository with significant star count and recent activity.

**Recency:** Very current, utilizing modern technologies like React 19 and Vite 6.

**Source:** [briehq/brie-extension/CLAUDE.md](https://github.com/briehq/brie-extension/blob/b18e550026e4acf322815bd91200692593397d91/CLAUDE.md) · 715★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Brie is a Chrome/Firefox/Edge/Safari browser extension for capturing screenshots, console errors, network issues, and user actions for bug reporting. It includes session recording (rrweb), video capture (FFmpeg WASM), and screenshot annotation (fabric.js).

## Commands

```bash
# Install dependencies
pnpm install --frozen-lockfile

# Development (Chrome)
pnpm run:chrome:local

# Development (Firefox)
pnpm run:firefox:local

# Production build
pnpm build:chrome:production
pnpm build:firefox:production

# Lint & format
pnpm lint
pnpm lint:fix
pnpm format

# Type checking
pnpm type-check

# Package extension
pnpm zip                  # Chrome
pnpm zip:firefox          # Firefox

# E2E tests
pnpm e2e

# Bump version across all packages
pnpm update-version
```

Command pattern: `pnpm <action>:<scope>:<env>` where action=`run|build`, scope=`chrome|firefox`, env=`local|production`.

## Architecture

This is a **pnpm monorepo** orchestrated by **Turborepo** with **Vite** as the build tool.

### Extension entry points (5 separate builds)

| Entry
```

</details>
