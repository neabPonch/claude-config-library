---
name: astashov__liftosaur
source: https://github.com/astashov/liftosaur/blob/068699c0de3387e1df74b5f535c4ddfbd228b125/CLAUDE.md
repo: astashov/liftosaur
kind: claude-md
stars: 597
last_pushed: 2026-06-14T23:36:16Z
license: agpl-3.0
score: 9
domains: [web-frontend, mobile-dev, automation-testing, ai-agents]
tags: [mcp-workflows, playwright, ios-simulator, coding-standards, architectural-context]
curated: 2026-06-15
curated_by: config-scout
---

# astashov/liftosaur — claude-md

**Why it's worth keeping:** The inclusion of exact MCP interaction workflows (including host calculation logic) and the 'comment-only-why' rule are exceptional examples of guiding agent behavior.

**Summary:** Provides detailed command sets and highly specific workflows for visual verification using Playwright and Mobile MCP. It also establishes strict coding standards and a structured knowledge management protocol.

**Source credibility:** High; based on a real, active project with highly specific domain-specific language (Liftoscript).

**Recency:** 

**Source:** [astashov/liftosaur/CLAUDE.md](https://github.com/astashov/liftosaur/blob/068699c0de3387e1df74b5f535c4ddfbd228b125/CLAUDE.md) · 597★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Starting Development
```bash
npm start          # Frontend dev server
npm run start:server  # Backend dev server with hot reload
```

### Building
```bash
npm run build      # Production build
npm run build:dev  # Development build
npm run build:lambda  # Build Lambda functions
```

### Testing & Quality
```bash
npm test           # Run all tests
npm run onetest    # Run single test file
npm run playwright # Run Playwright E2E tests
npm run lint       # ESLint for TypeScript files
```

### AWS Lambda Development
```bash
npm run start:lambda  # Local Lambda API
npm run watch:lambda  # Watch & rebuild Lambda
```

### iOS/watchOS Development
```bash
# Build watch bundle (included in build:dev, deployed to server)
npm run build:dev

# Watch bundle is downloaded from https://www.liftosaur.com/watch-bundle.js
# by WatchCacheManager at runtime - no manual copy needed

# Build watch app (run from ./ios)
xcodebuild -workspace Liftosaur.xcworkspace -scheme "LiftosaurWatch" -destination 'platform=watchOS Simulator,id=6D3DDA86-DDC2-4D24-8908-21839A09
```

</details>
