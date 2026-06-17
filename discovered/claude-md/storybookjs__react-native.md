---
name: storybookjs__react-native
source: https://github.com/storybookjs/react-native/blob/1f966228449dd54041dee54f3e3d83991b56fcbd/CLAUDE.md
repo: storybookjs/react-native
kind: claude-md
stars: 1294
last_pushed: 2026-06-14T20:54:29Z
license: mit
score: 8
domains: [mobile-development, react-native, monorepo]
tags: [react-native, storybook, pnpm, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# storybookjs/react-native — claude-md

**Why it's worth keeping:** It excels at explaining the logic behind build system configurations (Metro vs. Rspack), which helps agents avoid breaking critical import/bundling behaviors during refactors.

**Summary:** Provides a clear breakdown of development commands and a deep technical architecture overview for a complex React Native monorepo.

**Source credibility:** High; Storybook is an industry-standard tool with high star count and active maintenance.

**Recency:** Very recent, consistent with modern development workflows.

**Source:** [storybookjs/react-native/CLAUDE.md](https://github.com/storybookjs/react-native/blob/1f966228449dd54041dee54f3e3d83991b56fcbd/CLAUDE.md) · 1294★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
This file provides guidance to agents when working with code in this repository.

## Development Commands

```sh
# Initial Setup
pnpm install
pnpm build

# Development
pnpm dev        # Watch all packages for changes
pnpm example    # Run the expo example app with Storybook

# Story Generation
pnpm -F expo-example storybook-generate # Regenerate storybook.requires.ts

# Testing
pnpm test       # Run unit tests across all packages
pnpm test:ci    # Run tests in CI mode

# Code Quality
pnpm lint       # Run ESLint across the codebase
pnpm format:check   # Check Prettier formatting
pnpm format:fix     # Auto-fix Prettier formatting

# Documentation (from docs/ directory)
cd docs
pnpm start      # Start development server
pnpm build      # Build documentation
pnpm serve      # Serve built documentation
```

## Architecture Overview

**pnpm workspaces monorepo** containing React Native Storybook packages.

### Packages

**Apps**

- examples/expo-example - Expo example app showcasing Storybook
- docs - Documentation site for Storybook React Native

**Core:**

- `@storybook/react-native` - Main package providing Storybook functionality
- `@storybook/react-native-ui` - Full UI components f
```

</details>
