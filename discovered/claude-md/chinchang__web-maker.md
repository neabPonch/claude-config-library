---
name: chinchang__web-maker
source: https://github.com/chinchang/web-maker/blob/4b4c50d467bb6f5b8f530448b7becd06e0738bdd/CLAUDE.md
repo: chinchang/web-maker
kind: claude-md
stars: 2691
last_pushed: 2026-06-11T13:39:17Z
license: mit
score: 9
domains: [web-frontend, chrome-extension]
tags: [preact, architecture-guide, coding-standards, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# chinchang/web-maker — claude-md

**Why it's worth keeping:** The 'Coding Patterns' section is elite; it proactively prevents LLM errors by mandating specific layout components (Stack/VStack) and a single CSS file approach, while also detailing the critical postMessage communication logic.

**Summary:** This file acts as a comprehensive technical manual covering build commands, architectural mappings, and specific coding standards. It provides the exact context needed for an AI to navigate both high-level structure and low-level implementation details.

**Source credibility:** High-quality source with 2.6k stars and recent maintenance activity.

**Recency:** Highly relevant for modern agentic workflows like Claude Code.

**Source:** [chinchang/web-maker/CLAUDE.md](https://github.com/chinchang/web-maker/blob/4b4c50d467bb6f5b8f530448b7becd06e0738bdd/CLAUDE.md) · 2691★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Web-Maker is a blazing fast offline web playground that supports multiple preprocessors and offers both a Chrome extension and web app. The codebase is built with Preact and includes a comprehensive build system for both web and extension distributions.

## Development Commands

### Build & Development

- `npm run dev` - Start development server with hot reload
- `npm run build` - Production build using Preact CLI
- `npm start` - Start dev server with preview server (combines dev + gulp start-preview-server)
- `npm run start:all` - Start dev server + preview server + collab server

### Testing & Quality

- `npm test` - Run Jest tests (uses `tests/` directory with mocks in `tests/__mocks__/`)
- `npm run lint` - Run ESLint on src directory
- `npm run cypress` - Run end-to-end tests with Cypress
- `npm run cypress:open` - Open Cypress test runner interactively

### Build Distribution

- `gulp release` - Full production release (web app + extension)
- `gulp devRelease` - Development release
- `gulp buildExtension` - Build Chrome extension only

### I
```

</details>
