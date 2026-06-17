---
name: hackjutsu__Lepton
source: https://github.com/hackjutsu/Lepton/blob/a1b2c4f0ec268a9ee3979d0b4d3875d525542d73/CLAUDE.md
repo: hackjutsu/Lepton
kind: claude-md
stars: 10334
last_pushed: 2025-11-18T04:04:53Z
license: mit
score: 8
domains: [desktop-app, frontend, electron]
tags: [architecture-map, guardrails, tech-stack]
curated: 2026-06-15
curated_by: config-scout
---

# hackjutsu/Lepton — claude-md

**Why it's worth keeping:** The 'Architecture' section maps directory structures to specific responsibilities, which is vital for agentic navigation. The 'Important Guidelines' provide essential negative constraints to prevent common AI errors like modifying dependencies.

**Summary:** A highly structured guide that provides both technical commands and a functional mental model of the project structure.

**Source credibility:** High; the repository has over 10k stars, indicating a significant and well-established project.

**Recency:** Current; although the tech stack is slightly dated (Electron 13), the documentation style is perfectly optimized for modern agentic workflows.

**Source:** [hackjutsu/Lepton/CLAUDE.md](https://github.com/hackjutsu/Lepton/blob/a1b2c4f0ec268a9ee3979d0b4d3875d525542d73/CLAUDE.md) · 10334★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Lepton is a lean code snippet manager powered by GitHub Gist, built with Electron, React, and Redux. It provides a desktop application for managing and organizing code snippets with features like unlimited public/secret snippets, tagging, markdown/Jupyter notebook support, and GitHub Enterprise integration.

## Tech Stack

- **Framework**: Electron (desktop app)
- **Frontend**: React + Redux (with Redux Thunk for async actions, Redux Form for forms)
- **Build System**: Webpack + Babel (ES6 transpilation)
- **Styling**: Sass/SCSS
- **Code Editor**: CodeMirror (via react-codemirror)
- **Linting**: ESLint with Standard config
- **Dependencies**: Uses yarn package manager

## Key Commands

### Development
```bash
# Install dependencies
yarn install

# Development build and run
yarn build && yarn start

# Watch mode for development
yarn webpack-watch

# Production build
yarn webpack-prod
```

### Building & Distribution
```bash
# Create installer for current platform
yarn dist

# Platform-specific builds
yarn dist -m    # macOS
yarn dist -w    # Windo
```

</details>
