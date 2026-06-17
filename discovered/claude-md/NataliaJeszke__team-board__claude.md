---
name: NataliaJeszke__team-board__claude
source: https://github.com/NataliaJeszke/team-board/blob/244c12f451573dc50554df95b097f72f382f96d5/apps/frontend/CLAUDE.md
repo: NataliaJeszke/team-board
kind: claude-md
stars: 1
last_pushed: 2026-03-29T19:50:19Z
license: unknown
score: 9
domains: [web-frontend, angular]
tags: [angular, ngrx, typescript, architecture-patterns]
curated: 2026-06-17
curated_by: config-scout
---

# NataliaJeszke/team-board — claude-md

**Why it's worth keeping:** It defines strict patterns (the Facade pattern and Component templates) to prevent the LLM from writing code that violates the established architecture. It also provides essential path aliases to ensure accurate file imports.

**Summary:** A highly structured guide for an Angular/NgRx application that covers development workflows, directory intent, and architectural constraints.

**Source credibility:** Low star count, but the technical depth suggests a well-engineered, modern codebase.

**Recency:** 

**Source:** [NataliaJeszke/team-board/apps/frontend/CLAUDE.md](https://github.com/NataliaJeszke/team-board/blob/244c12f451573dc50554df95b097f72f382f96d5/apps/frontend/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Angular 21 task board application using NgRx for state management, PrimeNG for UI components, and Tailwind CSS for styling. This is a standalone component architecture (no NgModules) with centralized state management and i18n support (Polish/English).

## Development Commands

### Running the Application
```bash
npm start                    # Start dev server at http://localhost:4200
ng serve                     # Alternative to npm start
```

### Building
```bash
npm run build               # Production build (outputs to dist/)
npm run watch               # Development build with file watching
ng build                    # Direct Angular CLI build
```

### Testing
```bash
npm test                    # Run unit tests with Jest
npm run test:watch          # Run tests in watch mode
npm run test:coverage       # Run tests with coverage report
npm run test:coverage:open  # Run tests with coverage and open report in browser
npm run test:ci             # Run tests in CI mode (with coverage, maxWorkers=2)
npm run test:karma          # Run legacy Karma t
```

</details>
