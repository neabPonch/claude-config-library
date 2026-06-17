---
name: Countly__countly-server
source: https://github.com/Countly/countly-server/blob/6080fad9ed2fc0c9e192c7efaf1e3e42c3a0c6ff/CLAUDE.md
repo: Countly/countly-server
kind: claude-md
stars: 5874
last_pushed: 2026-06-15T08:34:06Z
license: other
score: 9
domains: [backend-api, web-frontend, security]
tags: [node.js, mongodb, plugin-architecture, security-first]
curated: 2026-06-15
curated_by: config-scout
---

# Countly/countly-server — claude-md

**Why it's worth keeping:** The 'Critical Security Rules' and 'Anti-Patterns' sections are gold; they prevent subtle logic errors (like missing app_id) that standard LLMs frequently miss. It also uses actual code templates to demonstrate how to interact with specific internal APIs.

**Summary:** Provides highly prescriptive technical guidelines, specific code boilerplates for API/Frontend integration, and critical security protocols essential for a plugin-based architecture.

**Source credibility:** High; Countly is a well-established, highly-starred open-source project with active maintenance.

**Recency:** Highly relevant for modern agentic workflows by providing explicit guardrails and structural context.

**Source:** [Countly/countly-server/CLAUDE.md](https://github.com/Countly/countly-server/blob/6080fad9ed2fc0c9e192c7efaf1e3e42c3a0c6ff/CLAUDE.md) · 5874★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Countly Server

This file provides guidance for Claude (Anthropic) when working with this codebase.

## Project Overview

Countly is a product analytics platform. Backend: Node.js 22+, MongoDB. Frontend: Vue 2, Element UI, Backbone (legacy). Architecture is plugin-based.

## Quick Commands

```bash
npm run start:all:dev        # Start all services (API:3001, Frontend:6001)
npx grunt dist-all           # Build static assets (required after JS changes)
npx grunt locales            # Build locale files
npx grunt sass               # Compile SASS only

# Testing
npm run test:unit            # Unit tests
npm run test:plugin -- name  # Single plugin tests
countly plugin lint name     # Lint plugin
countly shellcheck           # Validate shell scripts
```

## Critical Security Rules

**ALWAYS follow these - no exceptions:**

1. **API endpoints must use validation**:
   ```javascript
   const { validateRead, validateCreate, validateUpdate, validateDelete } = require('../../../api/utils/rights.js');
   validateRead(params, FEATURE_NAME, () => { /* handler */ });
   ```

2. **Write operations must include app_id**:
   ```javascript
   // CORRECT - prevents cross-app access
   d
```

</details>
