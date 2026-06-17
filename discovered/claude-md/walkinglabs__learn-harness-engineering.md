---
name: walkinglabs__learn-harness-engineering
source: https://github.com/walkinglabs/learn-harness-engineering/blob/51a6d701fe48aacfbdb0c1bb8cf34767fe012f5e/CLAUDE.md
repo: walkinglabs/learn-harness-engineering
kind: claude-md
stars: 8510
last_pushed: 2026-06-13T14:10:52Z
license: mit
score: 9
domains: [electron, typescript]
tags: [architecture, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# walkinglabs/learn-harness-engineering — claude-md

**Why it's worth keeping:** It defines 'Key Patterns' like IPC constant usage and dual tsconfig requirements to prevent process-boundary errors. It also creates a mental model of the relationship between Main, Preload, and Renderer processes.

**Summary:** Provides architectural blueprints and interaction patterns for a multi-process Electron application used in an educational context.

**Source credibility:** High; highly starred repository with very recent maintenance/activity.

**Recency:** Highly current, utilizing modern toolchains like VitePress, Vitest, and tsx.

**Source:** [walkinglabs/learn-harness-engineering/CLAUDE.md](https://github.com/walkinglabs/learn-harness-engineering/blob/51a6d701fe48aacfbdb0c1bb8cf34767fe012f5e/CLAUDE.md) · 8510★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Learn Harness Engineering is a project-based course on building reliable coding environments for AI agents. The repo contains a VitePress documentation site plus hands-on project code.

## Commands

```sh
# Documentation site
npm install
npm run docs:dev        # Dev server with hot reload (VitePress)
npm run docs:build      # Production build
npm run docs:preview    # Preview built site

# Run lecture code examples
npx tsx docs/lectures/<lecture-dir>/code/<file>.ts

# Project Electron apps (from each project directory)
cd projects/project-NN/starter  # or solution/
npm install
npm run dev              # Build + launch Electron (via scripts/dev.js)
npm run check            # Type-check both tsconfig.json and tsconfig.node.json
npm run test             # Vitest run (single run)
npm run test:watch       # Vitest watch mode
```

## Repository Structure

- `docs/` — VitePress documentation site (lectures, projects, resources)
- `docs/.vitepress/config.mts` — Nav/sidebar config for all 13 locales (en, zh, zh-TW, ja, ko, es, fr, ru, de, ar, vi, uz, tr)
```

</details>
