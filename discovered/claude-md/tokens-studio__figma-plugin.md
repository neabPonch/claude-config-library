---
name: tokens-studio__figma-plugin
source: https://github.com/tokens-studio/figma-plugin/blob/c831c61a305ef9baec7cdbf279f0a784dfe61ef6/CLAUDE.md
repo: tokens-studio/figma-plugin
kind: claude-md
stars: 1591
last_pushed: 2026-06-12T07:05:52Z
license: mit
score: 9
domains: [web-frontend, figma-plugin, monorepo]
tags: [architectural-context, monorepo-instructions, dual-thread]
curated: 2026-06-14
curated_by: config-scout
---

# tokens-studio/figma-plugin — claude-md

**Why it's worth keeping:** The breakdown of thread communication patterns (Main vs UI) and distinguishing package-specific commands from root commands are excellent patterns for AI guidance.

**Summary:** Provides exhaustive architectural context for a dual-thread Figma plugin within a Turbo monorepo.

**Source credibility:** High; based on a popular, actively maintained open-source project with significant stars.

**Recency:** Current; uses modern tooling like Turbo and SWC.

**Source:** [tokens-studio/figma-plugin/CLAUDE.md](https://github.com/tokens-studio/figma-plugin/blob/c831c61a305ef9baec7cdbf279f0a784dfe61ef6/CLAUDE.md) · 1591★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

This is a monorepo using Turbo and Yarn workspaces. The main Figma plugin is in `packages/tokens-studio-for-figma/`.

### Common Commands
- `yarn --frozen-lockfile --immutable` - Install dependencies
- `yarn build` - Build all packages 
- `yarn start` - Start development mode (runs webpack in watch mode)
- `yarn lint` - Run ESLint across all packages
- `yarn test` - Run Jest tests across all packages
- `yarn test:watch` - Run tests in watch mode

### Plugin-Specific Commands (run from `packages/tokens-studio-for-figma/`)
- `yarn build` - Production build with webpack
- `yarn build:dev` - Development build
- `yarn start` - Start webpack in development watch mode
- `yarn test` - Run Jest tests with feature flags enabled
- `yarn test:watch` - Run tests in watch mode without coverage
- `yarn test:coverage` - Run tests with coverage reporting
- `yarn cy:open` - Open Cypress for E2E testing
- `yarn cy:run` - Run Cypress tests headlessly
- `yarn lint` - Run ESLint with auto-fix
- `yarn lint:nofix` - Run ESLint without auto-fix
- `yarn storybook` - S
```

</details>
