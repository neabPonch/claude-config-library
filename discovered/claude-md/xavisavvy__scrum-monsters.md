---
name: xavisavvy__scrum-monsters
source: https://github.com/xavisavvy/scrum-monsters/blob/69bf286c8730bbb41af33d4af0d8eed151481c0c/CLAUDE.MD
repo: xavisavvy/scrum-monsters
kind: claude-md
stars: 3
last_pushed: 2026-06-08T13:20:13Z
license: other
score: 9
domains: [web-frontend, backend-api, real-time]
tags: [typescript, websocket, fullstack, game-dev]
curated: 2026-06-15
curated_by: config-scout
---

# xavisavvy/scrum-monsters — claude-md

**Why it's worth keeping:** It provides explicit 'how-to' workflows for extending functionality (like adding WebSocket events) and clarifies complex, non-obvious logic like how player avatars interact with game phases.

**Summary:** A highly detailed architectural guide that explains the game's state machine and real-time communication protocols. It covers full-stack development from local environment setup to Kubernetes deployment.

**Source credibility:** Active repository with high-quality, structured documentation typical of professional-grade full-stack projects.

**Recency:** Current; utilizes modern toolchains including Vite, Vitest, and Drizzle ORM.

**Source:** [xavisavvy/scrum-monsters/CLAUDE.MD](https://github.com/xavisavvy/scrum-monsters/blob/69bf286c8730bbb41af33d4af0d8eed151481c0c/CLAUDE.MD) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**ScrumQuest** is a real-time multiplayer scrum poker estimation game with JRPG-style boss battles. Full-stack TypeScript with Socket.IO for real-time sync and React Three Fiber for 3D graphics.

## Development Commands

```bash
npm run dev          # Start dev server (http://localhost:5000)
npm run build        # Production build (client + server)
npm run start        # Start production server
npm run check        # TypeScript type checking
npm run db:push      # Push Drizzle schema changes to database

# Testing (Vitest)
npm test             # Run all tests once
npm run test:watch   # Watch mode
npm run test:coverage # With coverage report

# Run a single test file
npx vitest run path/to/file.test.ts

# E2E Testing (Playwright)
npm run test:e2e     # Run E2E tests
npm run test:e2e:ui  # E2E tests with interactive UI

# Linting (ESLint)
npm run lint         # Check for issues
npm run lint:fix     # Auto-fix issues

# Releases (standard-version)
npm run release          # Auto-determine version bump
npm run release:patch    # Patch release (x.x.X
```

</details>
