---
name: cactuslab__capacitor-native-navigation
source: https://github.com/cactuslab/capacitor-native-navigation/blob/20c3b67df289bfe2489b83c352eea1ef3832fb97/CLAUDE.md
repo: cactuslab/capacitor-native-navigation
kind: claude-md
stars: 36
last_pushed: 2026-04-16T03:16:22Z
license: other
score: 9
domains: [mobile-development, monorepo-management, cross-platform]
tags: [capacitor, react-native-bridge, ios, android, pnpm]
curated: 2026-06-15
curated_by: config-scout
---

# cactuslab/capacitor-native-navigation — claude-md

**Why it's worth keeping:** Includes critical architectural mapping between JS and Native, platform-specific verification commands, and explicit warnings about known memory leak patterns.

**Summary:** A highly detailed guide for a complex cross-platform monorepo that bridges React with native iOS/Android components.

**Source credibility:** High; demonstrates specialized knowledge of the Capacitor ecosystem and recent activity.

**Recency:** Extremely current; references Node 22 and modern pnpm workspaces.

**Source:** [cactuslab/capacitor-native-navigation/CLAUDE.md](https://github.com/cactuslab/capacitor-native-navigation/blob/20c3b67df289bfe2489b83c352eea1ef3832fb97/CLAUDE.md) · 36★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Capacitor Native Navigation is a Capacitor plugin that lets React DOM apps use native navigation components (UINavigationController, UITabBarController on iOS; Fragments on Android). It bridges React views with native view controllers/fragments so each "screen" is a real native navigation entry.

## Monorepo Structure

pnpm workspace with packages in `packages/`:

- **`plugin`** (`capacitor-native-navigation`) — Core Capacitor plugin: TypeScript API, iOS Swift implementation, Android Kotlin implementation, web fallback
- **`react`** (`capacitor-native-navigation-react`) — React integration: view lifecycle, portal rendering, `initReact()`
- **`react-router`** (`capacitor-native-navigation-react-router`) — React Router 6 integration: custom Navigator, modal path matching
- **`history`** (`capacitor-native-navigation-history`) — Alternative integration using History API directly
- **`example`** — Example Vite + React app with iOS and Android native projects

## Build Commands

```shell
nvm use                  # Node 22
pnpm install             # In
```

</details>
