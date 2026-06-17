---
name: viap__dom-api
source: https://github.com/viap/dom-api/blob/0eee9769c255023e6aa134245e2b2eeae564e5b1/CLAUDE.md
repo: viap/dom-api
kind: claude-md
stars: 0
last_pushed: 2026-06-09T08:49:25Z
license: unknown
score: 9
domains: [backend-api, security, node-js]
tags: [nestjs, mongodb, architecture, procedural-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# viap/dom-api — claude-md

**Why it's worth keeping:** It includes actionable procedural guides like 'Adding a New Module' and explicitly lists global providers to prevent the AI from attempting redundant configurations.

**Summary:** This file provides deep architectural context for a NestJS/MongoDB project, including specific module creation workflows and security layers.

**Source credibility:** Low star count on GitHub, but the high density of technical detail suggests a professionally engineered project rather than a boilerplate.

**Recency:** Very current; specifically mentions Claude Code and follows modern TypeScript/NestJS patterns.

**Source:** [viap/dom-api/CLAUDE.md](https://github.com/viap/dom-api/blob/0eee9769c255023e6aa134245e2b2eeae564e5b1/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a NestJS-based REST API for a therapy/psychology practice management platform. The application manages psychologists, therapy sessions, therapy requests, users, bookings, and notifications — with WebSocket support for real-time communication.

## Development Commands

```bash
# Development
npm run start:dev          # Start in watch mode
npm run start:debug        # Start with debug mode

# Building
npm run build             # Build the application
npm run start:prod        # Run production build

# Testing
npm run test              # Run unit tests
npm run test:watch        # Run tests in watch mode
npm run test:e2e          # Run end-to-end tests
npm run test:cov          # Run tests with coverage

# Code Quality
npm run lint              # Run ESLint with auto-fix
npm run format            # Format code with Prettier
```

## Architecture

### Core Framework
- **NestJS**: TypeScript-based Node.js framework with decorators and dependency injection
- **MongoDB**: Database with Mongoose ODM
- **JWT Authentication**: Token-based auth with r
```

</details>
