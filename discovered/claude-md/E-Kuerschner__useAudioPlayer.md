---
name: E-Kuerschner__useAudioPlayer
source: https://github.com/E-Kuerschner/useAudioPlayer/blob/aa0fbe39c610855b1ce77f98dd208eae05a4ea91/CLAUDE.md
repo: E-Kuerschner/useAudioPlayer
kind: claude-md
stars: 353
last_pushed: 2026-05-28T03:17:16Z
license: unknown
score: 8
domains: [web-frontend, react-library]
tags: [monorepo, react, yarn-v4, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# E-Kuerschner/useAudioPlayer — claude-md

**Why it's worth keeping:** It bridges the gap between 'where files are' and 'how they work' by explaining design patterns like state synchronization, which prevents architectural drift during AI-driven edits.

**Summary:** Provides a clear map of a Yarn v4 monorepo, including specific build commands, workspace structures, and architectural patterns.

**Source credibility:** High; based on a popular, well-maintained React audio library with significant community traction.

**Recency:** Very current; includes modern tooling instructions for Yarn v4 and Corepack.

**Source:** [E-Kuerschner/useAudioPlayer/CLAUDE.md](https://github.com/E-Kuerschner/useAudioPlayer/blob/aa0fbe39c610855b1ce77f98dd208eae05a4ea91/CLAUDE.md) · 353★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Yarn v4 monorepo for the `react-use-audio-player` package, a React hook library for building custom audio playback controls. The package is built on top of Howler.js and provides React state synchronization with audio playback.

## Development Environment Setup

1. Use Node.js version specified in `.nvmrc` (v22.12.0)
2. Enable corepack: `corepack enable`
3. Install dependencies: `yarn install`
4. The project uses Yarn v4 with workspaces enabled

## Common Commands

### Building and Development
- `yarn g:build-package` - Build the react-use-audio-player package from anywhere in the monorepo
- `yarn workspace react-use-audio-player build` - Build the main package directly
- `yarn workspace react-use-audio-player build-watch` - Build in watch mode
- `yarn workspace react-use-audio-player lint` - TypeScript type checking (no ESLint, just `tsc`)

### Linting and Quality
- `yarn lint-all` - Run lint across all workspaces
- `yarn constraints` - Enforce Yarn workspace constraints

### Demo Applications
- `yarn workspace showcase start` - Run th
```

</details>
