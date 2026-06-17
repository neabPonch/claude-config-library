---
name: jitsi__lib-jitsi-meet
source: https://github.com/jitsi/lib-jitsi-meet/blob/3df0d953c62505fc589e282e88f6f5d20c77a02f/CLAUDE.md
repo: jitsi/lib-jitsi-meet
kind: claude-md
stars: 1414
last_pushed: 2026-06-15T18:44:23Z
license: apache-2.0
score: 9
domains: [web-frontend, video-api, javascript-library]
tags: [architecture, typescript-migration, build-system, integration-guide]
curated: 2026-06-15
curated_by: config-scout
---

# jitsi/lib-jitsi-meet — claude-md

**Why it's worth keeping:** Excellent use of module-specific commit scopes and explicit instructions for large-scale refactoring. The 'Integration' section is highly valuable for teaching an AI how to manage local dependencies in a mono-repo or multi-package setup.

**Summary:** Provides deep architectural context, detailed build/test workflows, and a clear roadmap for the ongoing JS-to-TS migration. It also explains complex local development integration workflows between interdependent packages.

**Source credibility:** High; a well-maintained, high-star industry standard library used for production video communications.

**Recency:** Very current; actively maintained and follows modern TypeScript/JavaScript development standards.

**Source:** [jitsi/lib-jitsi-meet/CLAUDE.md](https://github.com/jitsi/lib-jitsi-meet/blob/3df0d953c62505fc589e282e88f6f5d20c77a02f/CLAUDE.md) · 1414★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## lib-jitsi-meet Architecture

This is the JavaScript library for accessing Jitsi Meet server-side deployments. It provides WebRTC functionality, XMPP communication, and media handling for Jitsi Meet clients.

## Common Development Commands

### Build Commands
```bash
npm run build           # Full build (webpack UMD bundle + TypeScript compilation)
npm run build:webpack   # Build UMD bundle only for browser <script> tags
npm run build:webpack-dev # Development webpack bundle
npm run build:tsc       # TypeScript compilation only for ESM modules
npm run watch           # Development build with file watching
```

### Development Commands

**Testing:**
- `npm test` - Run all tests via Karma (single run)
- `npm run test-watch` - Run tests in watch mode
- Tests use Jasmine framework with Chrome headless browser

**Code Quality:**
- `npm run lint` - ESLint + TypeScript type checking
- `npm run lint-fix` - Auto-fix linting issues
- `npm run type-check` - TypeScript type checking only

**Documentation:**
- `npm run typedoc` - Generate TypeScript documentation

**Other:**
 -
```

</details>
