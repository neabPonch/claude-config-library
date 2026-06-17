---
name: expo__orbit
source: https://github.com/expo/orbit/blob/55d429f6e8f85b0655ed388b4275ec03d2703e68/CLAUDE.md
repo: expo/orbit
kind: claude-md
stars: 813
last_pushed: 2026-06-15T00:18:10Z
license: mit
score: 8
domains: [cli-tools, desktop-apps, monorepo]
tags: [monorepo, electron, react-native, yarn]
curated: 2026-06-15
curated_by: config-scout
---

# expo/orbit — claude-md

**Why it's worth keeping:** Excellent detail on cross-package workflow synchronization (e.g., the CLI update step) and clear command-level granularity per sub-directory.

**Summary:** Provides a comprehensive roadmap for navigating a complex monorepo, covering build commands, package dependencies, and specific development workflows.

**Source credibility:** Highly credible; maintained by Expo, a leading mobile developer tool organization.

**Recency:** Very current, referencing modern tech stacks like React 19 and TypeScript 5.8.

**Source:** [expo/orbit/CLAUDE.md](https://github.com/expo/orbit/blob/55d429f6e8f85b0655ed388b4275ec03d2703e68/CLAUDE.md) · 813★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Expo Orbit is a desktop menu bar application and CLI tool that accelerates mobile development workflows through one-click build launches and simulator/emulator management. It supports macOS, Windows, and Linux.

## Monorepo Structure

This is a Yarn/Lerna monorepo:
- **apps/cli** - Node.js CLI tool (expo-orbit-cli) using Commander.js
- **apps/menu-bar** - Main desktop app built with React Native + Electron
- **packages/common-types** - Shared TypeScript type definitions
- **packages/eas-shared** - Shared utilities for EAS, device management, app launching
- **packages/react-native-electron-modules** - Native Electron module bindings
- **packages/react-native-multi-window** - Multi-window management for Electron

## Build Commands

Root level commands (run from repo root):
```bash
yarn build        # Build all packages via Lerna
yarn lint         # Lint all packages
yarn watch        # Watch mode for all packages
yarn typecheck    # TypeScript type checking
```

### CLI App (apps/cli)
```bash
yarn build        # Compile TypeScript
yarn test
```

</details>
