---
name: minusxai__minusx-metabase
source: https://github.com/minusxai/minusx-metabase/blob/829bc9a539b8854c850b5707576c23cfa0c46e20/CLAUDE.md
repo: minusxai/minusx-metabase
kind: claude-md
stars: 348
last_pushed: 2026-06-12T09:48:06Z
license: mit
score: 9
domains: [web-frontend, browser-extensions, monorepos]
tags: [architecture, state-management, tribal-knowledge, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# minusxai/minusx-metabase — claude-md

**Why it's worth keeping:** The inclusion of 'CRITICAL' warnings captures vital tribal knowledge that LLMs cannot infer from source code alone. The detailed breakdown of cross-boundary communication patterns is highly transferable to any multi-package system.

**Summary:** Provides a high-density architectural map of a complex monorepo involving web apps and browser extensions. It bridges the gap between code structure and operational 'gotchas' like Redux state migrations.

**Source credibility:** High; the repo is well-starred and has very recent activity (0 months ago).

**Recency:** Current; follows modern monorepo and Chrome Extension V3 patterns.

**Source:** [minusxai/minusx-metabase/CLAUDE.md](https://github.com/minusxai/minusx-metabase/blob/829bc9a539b8854c850b5707576c23cfa0c46e20/CLAUDE.md) · 348★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Root Level Commands
- `yarn` - Install all dependencies for all workspaces
- `yarn web` - Start web development server
- `yarn web-prod` - Build and serve web app in production mode
- `yarn extension` - Start extension development server
- `yarn extension-build` - Build extension for production

### Workspace-Specific Commands
- **Web workspace**: `yarn lint`, `yarn test` (Jest), `yarn prettier`, `yarn build`
- **Extension workspace**: `yarn lint`, `yarn prettier`, `yarn zip` (build and package)
- **Apps workspace**: Jest tests available

## Architecture Overview

### Monorepo Structure
MinusX is organized as a yarn workspace monorepo with 3 main packages:

1. **`web/`** - React frontend application with Redux state management
2. **`extension/`** - Chrome extension with content scripts and background workers  
3. **`apps/`** - Platform-specific integrations, currently focused on Metabase

### Key Architectural Patterns

#### App Controller Pattern (`apps/`)
- Base class `AppController` in `apps/src/base/appController.ts` provides common f
```

</details>
