---
name: gre__react-native-view-shot
source: https://github.com/gre/react-native-view-shot/blob/2cd48ae2d06678bc843610acc3604725ff4462ec/CLAUDE.md
repo: gre/react-native-view-shot
kind: claude-md
stars: 2932
last_pushed: 2026-06-10T20:47:36Z
license: mit
score: 9
domains: [mobile-development, cross-platform]
tags: [architecture-mapping, build-workflows, platform-specifics]
curated: 2026-06-15
curated_by: config-scout
---

# gre/react-native-view-shot — claude-md

**Why it's worth keeping:** The 'Key Behaviors' section is gold; it documents critical implementation details like platform-specific quirks that prevent an AI from introducing breaking changes. It also provides clear command contexts for both the core library and its various example apps.

**Summary:** Provides a high-density technical map of a cross-platform library, covering build commands and complex multi-layer architecture.

**Source credibility:** High; a highly popular, well-maintained React Native industry standard.

**Recency:** Very current; includes modern details regarding TurboModules and the New Architecture.

**Source:** [gre/react-native-view-shot/CLAUDE.md](https://github.com/gre/react-native-view-shot/blob/2cd48ae2d06678bc843610acc3604725ff4462ec/CLAUDE.md) · 2932★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

`react-native-view-shot` is a React Native library (v4.0+) for capturing React Native views as images. It supports iOS, Android, Windows, and Web, and is compatible with both the old and new React Native architectures (Fabric + TurboModules).

## Commands

### Library (root)

```bash
npm run build          # Compile TypeScript → lib/
npm run type-check     # Type-check without emitting
npm run lint           # ESLint
npm run lint:ci        # ESLint (zero warnings allowed)
npm run format         # Prettier format
npm run format:check   # Check formatting
```

### Example App (cd example)

```bash
npm run ios            # Run on iOS simulator
npm run android        # Run on Android emulator
npm run start          # Start Metro bundler

# E2E tests (Detox)
npm run build:e2e:ios
npm run test:e2e:ios
UPDATE_SNAPSHOTS=true npm run test:e2e:ios   # Regenerate reference snapshots

npm run build:e2e:android
npm run test:e2e:android
UPDATE_SNAPSHOTS=true npm run test:e2e:android
```

## Architecture

### JS/TS Layer (`src/`)

- **`src/index.tsx`** — Main e
```

</details>
