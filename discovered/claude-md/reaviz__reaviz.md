---
name: reaviz__reaviz
source: https://github.com/reaviz/reaviz/blob/cde88e9722fe8e2badd5d5eced20f25ac89a9847/CLAUDE.md
repo: reaviz/reaviz
kind: claude-md
stars: 1236
last_pushed: 2026-06-12T18:42:13Z
license: apache-2.0
score: 9
domains: [web-frontend, data-visualization, react]
tags: [typescript, react, d3, storybook]
curated: 2026-06-15
curated_by: config-scout
---

# reaviz/reaviz — claude-md

**Why it's worth keeping:** Uses explicit code snippets to define component patterns, import aliasing, and styling protocols, which prevents AI from inventing its own styles. The detailed directory tree and command list provide immediate operational utility.

**Summary:** A highly structured guide for a React/D3 library that provides deep architectural context and strict coding standards.

**Source credibility:** High-quality open source project with significant stars and recent maintenance.

**Recency:** Current; reflects modern development workflows using Vitest, Storybook v9, and TypeScript.

**Source:** [reaviz/reaviz/CLAUDE.md](https://github.com/reaviz/reaviz/blob/cde88e9722fe8e2badd5d5eced20f25ac89a9847/CLAUDE.md) · 1236★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for REAVIZ

## Project Overview

REAVIZ is a modular React charting library that uses D3.js for calculations and React for rendering. It provides a composable API for building data visualizations with features like animations, tooltips, legends, and accessibility support.

- **Repository**: https://github.com/reaviz/reaviz
- **License**: Apache-2.0
- **Node Version**: >=22
- **Package Manager**: npm (>=10.8.2)

## Quick Reference Commands

```bash
# Install dependencies
npm install

# Development (Storybook)
npm start                  # Start Storybook dev server on port 9009

# Build
npm run build              # Full build (JS + docs)
npm run build:js           # Build library only (Vite)
npm run build-storybook    # Build Storybook static site

# Testing
npm test                   # Run tests with Vitest (watch mode)
npm run test:ci            # Run tests with coverage
npm run test-storybook     # Run Storybook visual tests

# Linting & Formatting
npm run lint               # Run ESLint
npm run lint:fix           # Run ESLint with auto-fix
npm run prettier           # Format code with Prettier
npm run ts:check           # TypeScript type checking
```

</details>
