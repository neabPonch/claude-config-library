---
name: zextras__carbonio-mails-ui
source: https://github.com/zextras/carbonio-mails-ui/blob/9c17e26c75e6031e65d19655897347e844c58de7/CLAUDE.md
repo: zextras/carbonio-mails-ui
kind: claude-md
stars: 11
last_pushed: 2026-06-12T15:02:19Z
license: agpl-3.0
score: 9
domains: [web-frontend, react]
tags: [react, vitest, zustand, microfrontend]
curated: 2026-06-15
curated_by: config-scout
---

# zextras/carbonio-mails-ui — claude-md

**Why it's worth keeping:** It explicitly documents complex state management patterns (task queues/sync handlers) and provides crucial path alias and testing setup information to prevent import errors.

**Summary:** A comprehensive architectural blueprint for a React-based mail module that details its integration within a larger host shell environment.

**Source credibility:** High; an enterprise-grade professional repository from Zextras with recent maintenance.

**Recency:** Very current, utilizing modern toolchains like Vitest, Playwright, and Zustand.

**Source:** [zextras/carbonio-mails-ui/CLAUDE.md](https://github.com/zextras/carbonio-mails-ui/blob/9c17e26c75e6031e65d19655897347e844c58de7/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Carbonio Mails UI is the mail module for the Zextras Carbonio webmail platform. It is a React-based microfrontend that runs inside the Carbonio Shell (`@zextras/carbonio-shell-ui`). It uses Emotion for styling and the Carbonio Design System (`@zextras/carbonio-design-system`) for UI components.

## Common Commands

```bash
npm install                  # Install dependencies
npm run start -- -h <host>   # Watch mode (host = Carbonio server for proxying)
npm run build                # Production build via carbonio-ui-sdk
npm run lint                 # ESLint (errors + warnings)
npm run lint-fix             # ESLint auto-fix
npm run lint-errors          # ESLint errors only (no warnings)
npm run type-check           # TypeScript type checking (tsc --noEmit)
npm run lint-check           # lint-errors + type-check combined

# Unit tests (vitest, jsdom, TZ=Europe/Rome)
npm test                              # Run all unit tests once
npx vitest run --project=unit <path>  # Run a single test file
npx vitest --project=unit <path>      # Watch mode for a si
```

</details>
