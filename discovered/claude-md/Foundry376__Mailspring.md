---
name: Foundry376__Mailspring
source: https://github.com/Foundry376/Mailspring/blob/b29ea0e65c4794eb6531134992d5fb19e2e02abd/CLAUDE.md
repo: Foundry376/Mailspring
kind: claude-md
stars: 17614
last_pushed: 2026-06-13T20:30:13Z
license: gpl-3.0
score: 10
domains: [desktop-app, electron, typescript]
tags: [architecture, sync-engine, data-flow, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# Foundry376/Mailspring — claude-md

**Why it's worth keeping:** Includes crucial warnings about dual source directories and uses ASCII diagrams to explain complex cross-process data flows. It explicitly defines invariants (e.g., read-only UI) that prevent the LLM from suggesting invalid database writes.

**Summary:** A high-density architectural guide detailing an Electron/C++ hybrid system, specifically focusing on the task-based sync engine and reactive database patterns.

**Source credibility:** High; Mailspring is a major, well-maintained open-source project with significant star count.

**Recency:** Current; provides relevant context for modern TypeScript/Electron development.

**Source:** [Foundry376/Mailspring/CLAUDE.md](https://github.com/Foundry376/Mailspring/blob/b29ea0e65c4794eb6531134992d5fb19e2e02abd/CLAUDE.md) · 17614★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Development Commands

```bash
# Install dependencies
npm install

# Run the app in development mode (uses --dev flag, data stored in Mailspring-dev folder)
npm start

# Run with specific language locale
npm start -- --lang=de

# Run linting (prettier + eslint)
npm run lint

# Run all tests
npm test

# Run window-specific tests
npm test-window

# TypeScript type checking in watch mode
npm run tsc-watch

# Build for production
npm run build
```

## Architecture Overview

Mailspring is an Electron-based email client written in TypeScript with React. It uses a plugin architecture where features are implemented as internal packages.

### Key Directories

- **`app/src/`** - Core application source code
  - `browser/` - Main process code (application lifecycle, window management, auto-updates)
  - `flux/` - Flux-based state management (actions, stores, models, tasks)
  - `components/` - Reusable React UI components
  - `services/` - Application services (search, sanitization, etc.)
  - `registries/` - Extension registries (components, extensions, database objec
```

</details>
