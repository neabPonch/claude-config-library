---
name: tonkeeper__tonkeeper-web
source: https://github.com/tonkeeper/tonkeeper-web/blob/54ea16f619bc09906246249a4ac47414ee6b09fa/CLAUDE.md
repo: tonkeeper/tonkeeper-web
kind: claude-md
stars: 429
last_pushed: 2026-06-12T14:56:04Z
license: apache-2.0
score: 10
domains: [web, crypto, monorepo]
tags: [monorepo, architecture-patterns, type-safety, platform-abstraction]
curated: 2026-06-15
curated_by: config-scout
---

# tonkeeper/tonkeeper-web — claude-md

**Why it's worth keeping:** It enforces strict interaction constraints (like using enums for storage keys) and explains the cross-package dependency graph to prevent build errors.

**Summary:** Provides deep architectural context for a complex monorepo, including platform abstraction patterns and state management rules.

**Source credibility:** High; maintained repository with 400+ stars and very recent activity.

**Recency:** Highly current, updated within the last month.

**Source:** [tonkeeper/tonkeeper-web/CLAUDE.md](https://github.com/tonkeeper/tonkeeper-web/blob/54ea16f619bc09906246249a4ac47414ee6b09fa/CLAUDE.md) · 429★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository overview

Yarn 4 monorepo with Turborepo for a non-custodial TON blockchain wallet. Two shared packages feed six platform apps:

- **`packages/core`** — business logic, API clients, crypto services, account model (no React)
- **`packages/uikit`** — all React components, state hooks, pages (depends on core)
- **`packages/locales`** — i18n translation files
- **`apps/web`** — Vite SPA
- **`apps/extension`** — Chrome/Firefox browser extension (MV2 for Firefox, MV3 for Chrome)
- **`apps/desktop`** — Electron app via `electron-forge`
- **`apps/twa`** — Telegram Mini App (Vite)
- **`apps/mobile`** — Capacitor iPad app (Vite)
- **`apps/web-swap-widget`** — embeddable swap widget (Vite)

## Common commands

```sh
# Install dependencies
yarn

# Development (web only)
yarn dev:web

# Build a specific app
yarn build:web
yarn build:extension
yarn build:desktop
yarn build:twa

# Build shared packages only (required before building apps manually)
npx turbo build:pkg

# Unit tests (run from packages/core)
yarn workspace @tonkeeper/core test

# Run a single test file
y
```

</details>
