---
name: tloncorp__tlon-apps
source: https://github.com/tloncorp/tlon-apps/blob/6249441648d89516764de63fac74ba7b8131ab5d/CLAUDE.md
repo: tloncorp/tlon-apps
kind: claude-md
stars: 103
last_pushed: 2026-06-17T01:12:48Z
license: mit
score: 9
domains: [web-frontend, backend-api, agents-ai]
tags: [monorepo, hoon, architecture-guide, mobile-desktop]
curated: 2026-06-17
curated_by: config-scout
---

# tloncorp/tlon-apps — claude-md

**Why it's worth keeping:** Implements 'negative constraints' to prevent common logical errors and provides exact implementation details for highly specialized, non-standard architectural patterns.

**Summary:** Provides complete development command sets and deep technical specifications for Hoon agent patterns and platform-specific UI navigation.

**Source credibility:** High; actively maintained repository with significant domain expertise in the Urbit/Hoon ecosystem.

**Recency:** Current; uses modern toolchains like pnpm, Vite, Tamagui, and Expo.

**Source:** [tloncorp/tlon-apps/CLAUDE.md](https://github.com/tloncorp/tlon-apps/blob/6249441648d89516764de63fac74ba7b8131ab5d/CLAUDE.md) · 103★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Building

-   `pnpm run build:all` - Build all packages and applications
-   `pnpm run build:packages` - Build shared packages only (shared, ui, editor)
-   `pnpm run build:web` - Build web application
-   `pnpm run build:mobile` - Build mobile application
-   `pnpm run build:desktop` - Build desktop application

### Development

-   `pnpm run dev:web` - Start web development server
-   `pnpm run dev:ios` - Start iOS development with live reload
-   `pnpm run dev:android` - Start Android development with live reload
-   `pnpm run dev:desktop` - Start desktop development

### Testing

-   `pnpm run test` - Run all tests with updates
-   `pnpm run test:ci` - Run all tests in CI mode
-   `pnpm run e2e` - Run end-to-end tests (web)
-   **E2E tests must be run from `apps/tlon-web` directory**: `cd apps/tlon-web && pnpm e2e:test <filename>`
    -   Use just the filename, NOT the full path: `channel-details.spec.ts` (correct) vs `e2e/channel-details.spec.ts` (wrong)
    -   Example: `cd apps/tlon-web && pnpm e2e:test channel-details.spec.ts`

##
```

</details>
