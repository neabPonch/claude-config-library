---
name: RocketChat__Rocket.Chat.ReactNative
source: https://github.com/RocketChat/Rocket.Chat.ReactNative/blob/1dfd2d4f10d449ba8d217564dc266a75a63832e7/CLAUDE.md
repo: RocketChat/Rocket.Chat.ReactNative
kind: claude-md
stars: 2390
last_pushed: 2026-06-15T17:28:17Z
license: mit
score: 9
domains: [mobile-development, react-native, frontend]
tags: [react-native, redux-saga, architecture, offline-first]
curated: 2026-06-15
curated_by: config-scout
---

# RocketChat/Rocket.Chat.ReactNative — claude-md

**Why it's worth keeping:** It explicitly distinguishes between state management patterns (Redux vs Zustand) and provides path-specific context for core systems like the database and API layers, preventing architectural drift.

**Summary:** A high-density technical manual that maps out complex architectural boundaries and specific command workflows for a large React Native app.

**Source credibility:** High-quality open-source project with significant stars and active maintenance.

**Recency:** Extremely current, referencing React 19 and Expo 54.

**Source:** [RocketChat/Rocket.Chat.ReactNative/CLAUDE.md](https://github.com/RocketChat/Rocket.Chat.ReactNative/blob/1dfd2d4f10d449ba8d217564dc266a75a63832e7/CLAUDE.md) · 2390★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Rocket.Chat React Native mobile client. Single-package React Native app (not a monorepo) using pnpm (version pinned in `package.json#packageManager`, activated via corepack). Supports iOS 13.4+ and Android 6.0+.

- React 19.1, React Native 0.81, Expo 54
- TypeScript with strict mode, baseUrl set to `app/` (imports resolve from there)
- Node: engines `>=18`, volta pins 24.13.1
- Read UBIQUITOUS_LANGUAGE.md

## Commands

```bash
# First-time setup (per machine)
corepack enable            # Activates the pnpm version pinned in package.json

# Install & setup
pnpm install               # Install dependencies (postinstall runs patch-package)
pnpm pod-install           # Install iOS CocoaPods (required before iOS builds)

# Run
pnpm start                 # Start Metro bundler
pnpm ios                   # Build and run on iOS
pnpm android               # Build and run on Android

# Test
TZ=UTC pnpm test           # Run Jest unit tests (TZ=UTC is set in script)
pnpm test --testPathPattern='path/to/test'  # Run a single test file
pnpm test-update
```

</details>
