---
name: jitsi__jitsi-meet
source: https://github.com/jitsi/jitsi-meet/blob/de045aa9e20db3b0581bc3b343e5bf05e978faad/CLAUDE.md
repo: jitsi/jitsi-meet
kind: claude-md
stars: 29413
last_pushed: 2026-06-13T04:50:37Z
license: apache-2.0
score: 9
domains: [web-frontend, mobile-app, cross-platform]
tags: [typescript, redux, react-native, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# jitsi/jitsi-meet — claude-md

**Why it's worth keeping:** It defines specific filename patterns (.web.ts vs .native.ts) and explains the custom Redux registry pattern, which prevents an AI from hallucinating standard Redux implementations instead of the project's unique one.

**Summary:** A highly detailed guide for a complex multi-platform codebase using feature-driven architecture and platform-specific file extensions.

**Source credibility:** Very high; Jitsi Meet is a major, mature open-source project with massive star count and active maintenance.

**Recency:** Current; the repository shows very recent activity.

**Source:** [jitsi/jitsi-meet/CLAUDE.md](https://github.com/jitsi/jitsi-meet/blob/de045aa9e20db3b0581bc3b343e5bf05e978faad/CLAUDE.md) · 29413★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Building and Development
- `npm run lint-fix` - Automatically fix linting issues
- `npm run tsc:ci` - Run TypeScript checks for both web and native platforms
- `npm run tsc:web` - TypeScript check for web platform only
- `npm run tsc:native` - TypeScript check for native platform only
- `npm run lint:ci` - Run ESLint without type checking
- `make dev` - Start development server with webpack-dev-server
- `make compile` - Build production bundles
- `make clean` - Clean build directory
- `make all` - Full build (compile + deploy)

### Testing
- `npm test` - Run full test suite using WebDriverIO
- `npm run test-single -- <spec-file>` - Run single test file
- `npm run test-dev` - Run tests against development environment
- `npm run test-dev-single -- <spec-file>` - Run single test in dev mode


### Language Tools
- `npm run lang-sort` - Sort language files
- `npm run lint:lang` - Validate JSON language files

### Platform-Specific TypeScript
TypeScript configuration is split between web and native platforms with separate tsconfig files.

## Ar
```

</details>
