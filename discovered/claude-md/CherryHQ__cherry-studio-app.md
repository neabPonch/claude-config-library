---
name: CherryHQ__cherry-studio-app
source: https://github.com/CherryHQ/cherry-studio-app/blob/1167eabbd5a8bacc27759ca9cb9c0dc1c1776b74/CLAUDE.md
repo: CherryHQ/cherry-studio-app
kind: claude-md
stars: 3450
last_pushed: 2026-06-14T02:39:29Z
license: agpl-3.0
score: 9
domains: [mobile-app, react-native, ai-integration]
tags: [expo, drizzle-orm, redux-toolkit, architecture-pattern]
curated: 2026-06-15
curated_by: config-scout
---

# CherryHQ/cherry-studio-app — claude-md

**Why it's worth keeping:** Includes specific implementation patterns for logging, database migrations, and the React Compiler; directs the LLM to specialized documentation for deep schema understanding.

**Summary:** A highly structured guide for a complex React Native/Expo AI application that covers architectural layers and operational workflows.

**Source credibility:** High: 3.4k stars and active maintenance suggest a professional-grade repository.

**Recency:** 

**Source:** [CherryHQ/cherry-studio-app/CLAUDE.md](https://github.com/CherryHQ/cherry-studio-app/blob/1167eabbd5a8bacc27759ca9cb9c0dc1c1776b74/CLAUDE.md) · 3450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Core Development

- `pnpm start` - Start Expo development server
- `pnpm android` - Run on Android device/emulator
- `pnpm ios` - Run on iOS device/simulator
- `pnpm prebuild` - Generate native code (required before first native run)

### Database

- `npx drizzle-kit generate` - Generate database migrations (required before first app run)
- `npx drizzle-kit studio` - Open Drizzle Studio for database inspection

### Code Quality

- `pnpm lint` - Run ESLint with auto-fix
- `pnpm format` - Run Prettier and ESLint formatting
- `pnpm test` - Run Jest tests with watch mode
- `pnpm check:i18n` - Validate internationalization files for missing translations
- `pnpm sync:i18n` - Sync translation keys across all language files

## Architecture Overview

Cherry Studio is a React Native/Expo AI chat application with clean architecture principles:

### Data Layer

- **SQLite + Drizzle ORM**: Type-safe database operations with schema-first approach
- **Redux Toolkit**: State management with persistence via AsyncStorage
- **MMKV**: High-performance key-v
```

</details>
