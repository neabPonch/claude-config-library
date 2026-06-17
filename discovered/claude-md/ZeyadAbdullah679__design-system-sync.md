---
name: ZeyadAbdullah679__design-system-sync
source: https://github.com/ZeyadAbdullah679/design-system-sync/blob/de58b32c6ba1cbb1ae1ad6ee90ce2ed6ac198a4f/CLAUDE.md
repo: ZeyadAbdullah679/design-system-sync
kind: claude-md
stars: 7
last_pushed: 2026-04-09T04:24:47Z
license: mit
score: 9
domains: [figma-plugin, design-systems, automation]
tags: [figma, typescript, design-tokens, esbuild]
curated: 2026-06-15
curated_by: config-scout
---

# ZeyadAbdullah679/design-system-sync — claude-md

**Why it's worth keeping:** It highlights critical environmental constraints (like the absence of native `btoa` and untestable extractors) that prevent an agent from attempting invalid operations. The clear mapping of source modules to their functional roles facilitates efficient navigation.

**Summary:** This file provides a detailed breakdown of the plugin's architecture, build system, and multi-platform export logic. It serves as an excellent technical guide for navigating a specialized Figma development environment.

**Source credibility:** High; it is a real-world tool with recent maintenance activity (2 months ago).

**Recency:** Current; updated very recently in 2024/2025 context.

**Source:** [ZeyadAbdullah679/design-system-sync/CLAUDE.md](https://github.com/ZeyadAbdullah679/design-system-sync/blob/de58b32c6ba1cbb1ae1ad6ee90ce2ed6ac198a4f/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Design System Sync is a Figma plugin that exports design tokens (strings/localization, colors, typography) from Figma to GitHub repositories. It generates platform-specific files for Android, iOS, Flutter, and Kotlin Multiplatform (KMP).

## Commands

```bash
npm install           # Install dependencies
npm run build         # Bundle src/ → code.js + ui.html via esbuild
npm run watch         # Build with file watching
npm run typecheck     # TypeScript type checking (no emit)
npm run clean         # Remove build artifacts (code.js, code.js.map, ui.html)
npm test              # Run all tests
npm run test:watch    # Run tests in watch mode
npm run test:coverage # Tests with coverage (50% min threshold)
npm run lint          # ESLint on src/
npm run lint:fix      # Auto-fix lint issues
```

To run a single test file: `npx jest tests/core/colorParsing.test.ts`

## Architecture

The plugin has two runtime components communicating via `figma.ui.postMessage` / `figma.ui.onmessage`. esbuild bundles the modular source files into two output artifacts that
```

</details>
