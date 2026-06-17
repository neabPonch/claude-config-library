---
name: vmurin__react-native-azure-auth
source: https://github.com/vmurin/react-native-azure-auth/blob/35e08290892ad9763068d1db98725f3dfd4a3055/CLAUDE.md
repo: vmurin/react-native-azure-auth
kind: claude-md
stars: 88
last_pushed: 2026-06-09T16:18:50Z
license: mit
score: 9
domains: [mobile-development, authentication-security]
tags: [react-native, oauth2, architecture-mapping]
curated: 2026-06-16
curated_by: config-scout
---

# vmurin/react-native-azure-auth — claude-md

**Why it's worth keeping:** The 'Architecture' section acts as a mental map that explains module responsibilities and data flow rather than just listing files. It also provides granular test commands which are essential for Claude Code's tool-use capabilities.

**Summary:** Provides a detailed functional breakdown of subsystems and specific command patterns for test execution.

**Source credibility:** High; well-maintained specialized library with active commits.

**Recency:** Very current; highly optimized for modern AI coding workflows.

**Source:** [vmurin/react-native-azure-auth/CLAUDE.md](https://github.com/vmurin/react-native-azure-auth/blob/35e08290892ad9763068d1db98725f3dfd4a3055/CLAUDE.md) · 88★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

React Native library implementing Azure AD OAuth2 V2.0 authentication. Provides token cache, authorization code grant with PKCE, silent token acquisition, and MS Graph API requests. Uses native modules (`SFSafariViewController` on iOS, Chrome Custom Tabs on Android) for the auth browser flow.

## Commands

- **Run all tests:** `yarn test` (or `npm test`) — runs Jest
- **Run a single test file:** `npx jest src/token/__tests__/scope.spec.js`
- **Run tests matching a name:** `npx jest -t "test name pattern"`

There is no separate build step — the library ships plain JS (ES modules with Babel transforms at consumer side). No lint script is configured in package.json; ESLint config exists at `.eslintrc.js`.

## Architecture

Entry point: `src/index.js` — exports the `AzureAuth` class, which composes two main subsystems:

- **`Auth`** (`src/auth/index.js`) — Core authentication logic. Builds authorize/logout URLs, exchanges authorization codes for tokens, refreshes tokens, performs silent token acquisition via cache, and wraps MS Graph API calls. Uses
```

</details>
