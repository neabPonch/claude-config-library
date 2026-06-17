---
name: antonycourtney__tabli
source: https://github.com/antonycourtney/tabli/blob/699132cb67a87f0e945294aee340b7365f730d8c/CLAUDE.md
repo: antonycourtney/tabli
kind: claude-md
stars: 410
last_pushed: 2025-09-27T23:50:38Z
license: mit
score: 7
domains: [web-extension, frontend]
tags: [react, typescript, chrome-extension, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# antonycourtney/tabli — claude-md

**Why it's worth keeping:** The 'Architecture' section is high value because it explains the indirect state update flow (UI -> client -> service worker), preventing the AI from attempting to manage state locally.

**Summary:** Defines build commands, strict TypeScript coding conventions, and the specific message-passing architecture for a Chrome extension.

**Source credibility:** Solid open-source project with 400+ stars and clear, manual documentation.

**Recency:** Current; reflects modern Chrome Extension/React patterns.

**Source:** [antonycourtney/tabli/CLAUDE.md](https://github.com/antonycourtney/tabli/blob/699132cb67a87f0e945294aee340b7365f730d8c/CLAUDE.md) · 410★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tabli Development Guide

## Commands
- Build: `npm run build-dev` (development) or `npm run build-prod` (production)
- Test: `npm run test` (run all tests)
- Test single file: `npx jest __tests__/tabWindowTest.ts`
- Lint: `npm run lint` (check) or `npm run lintfix` (auto-fix)
- Watch: `npm run watch` (development) or `npm run watch-prod` (production)
- Storybook: `npm run storybook`

## Code Style
- TypeScript with React functional components and hooks
- 2-space indentation, no max line length
- Use PascalCase for components (FilteredTabWindowUI)
- Use camelCase for utils and non-components (tabWindowUtils)
- Components in .tsx files, utilities in .ts files
- Favor immutable state patterns (Immer used extensively)
- Use type definitions rather than interfaces where possible
- Error handling with try/catch blocks and loglevel library
- Tests use Jest with snapshot testing

## Architecture
- Chrome extension with popup and background contexts
- State managed in service worker running in background
- UI components should update state by calling functions in `actionsClient.ts`
- `actionsClient.ts` sends messages to service worker
- Service worker handles these messages in `actionsSer
```

</details>
