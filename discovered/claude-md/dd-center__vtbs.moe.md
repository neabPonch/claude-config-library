---
name: dd-center__vtbs.moe
source: https://github.com/dd-center/vtbs.moe/blob/d9a53593749c1b435a4efac371f4e2752c17f264/CLAUDE.md
repo: dd-center/vtbs.moe
kind: claude-md
stars: 632
last_pushed: 2025-07-31T13:39:09Z
license: mit
score: 8
domains: [backend-api, web-frontend, real-time-systems]
tags: [vue2, nodejs-cluster, websocket, leveldb, architecture-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# dd-center/vtbs.moe — claude-md

**Why it's worth keeping:** The inclusion of 'Critical Notes' regarding version-specific constraints (Vue 2 vs 3) and the 'Process Architecture' section prevents LLM hallucination in multi-process environments.

**Summary:** Provides a highly structured architectural map covering process orchestration, data flow, and specific command workflows.

**Source credibility:** Solid mid-sized project with clear architectural documentation for a niche domain.

**Recency:** Highly relevant; though the repo is older, the structural pattern of guiding an agent through complex system flows remains modern.

**Source:** [dd-center/vtbs.moe/CLAUDE.md](https://github.com/dd-center/vtbs.moe/blob/d9a53593749c1b435a4efac371f4e2752c17f264/CLAUDE.md) · 632★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

vtbs.moe is a real-time VTuber monitoring platform for Bilibili streamers, combining Vue.js frontend with Node.js cluster-based backend, WebSocket communication, and LevelDB persistence.

## Development Commands

### Setup and Dependencies
```bash
git submodule update --init --recursive  # Initialize submodules (required)
npm install                               # Install dependencies
```

### Development Workflow
```bash
npm run serve                            # Frontend dev server with hot reload
npm run dev                              # Compile TypeScript in watch mode
npm run tsc                              # Compile TypeScript once
npm run build                            # Full production build (tsc + vue build)
npm run lint                             # Lint Vue components
npm run test                             # Run tests (alias for build)
```

### Backend Development
```bash
node api/mock                            # Run with mocked external services
node index.cjs                           # Run full backend (requires external dep
```

</details>
