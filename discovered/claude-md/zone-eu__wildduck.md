---
name: zone-eu__wildduck
source: https://github.com/zone-eu/wildduck/blob/0e169013d6c8cfeba4677e5538a375fbb4a97f3d/CLAUDE.md
repo: zone-eu/wildduck
kind: claude-md
stars: 2096
last_pushed: 2026-06-12T08:11:27Z
license: eupl-1.2
score: 9
domains: [backend, node.js, distributed-systems]
tags: [architecture-patterns, data-flow, protocol-implementation]
curated: 2026-06-15
curated_by: config-scout
---

# zone-eu/wildduck — claude-md

**Why it's worth keeping:** Includes specific code snippets of internal design patterns (like the async handler pattern) and detailed state machine logic that prevents AI hallucination during implementation.

**Summary:** Provides deep architectural context for a complex mail server ecosystem, including internal coding patterns and high-level data flows between services.

**Source credibility:** High: 2000+ stars and actively maintained.

**Recency:** Highly current; utilizes high-density context structure ideal for modern agentic tools.

**Source:** [zone-eu/wildduck/CLAUDE.md](https://github.com/zone-eu/wildduck/blob/0e169013d6c8cfeba4677e5538a375fbb4a97f3d/CLAUDE.md) · 2096★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

WildDuck is a scalable, no-SPOF IMAP/POP3 mail server built with Node.js. It uses MongoDB for storage (with sharding/replication support), Redis for pubsub/caching, and provides a comprehensive REST API for management.

**Dual Role**: WildDuck serves as both a standalone application AND a library. External mail components (Haraka, ZoneMTA) import WildDuck's handlers via `@zone-eu/wildduck/lib/*` to share the same database and business logic.

## Common Commands

```bash
# Run all tests (drops test DB, flushes Redis, then runs tests)
npm test

# Run protocol tests only (no MongoDB required)
npm run test:proto

# Run tests without DB cleanup
npm run runtest

# Show effective configuration
npm run printconf

# Start the server
npm start

# Generate API documentation
npm run apidoc
```

### Running Individual Tests

```bash
# Unit tests (no server needed)
NODE_ENV=test ./node_modules/.bin/mocha imap-core/test/imap-parser-unit.js

# API tests (requires server running separately: node server.js)
NODE_ENV=test ./node_modules/.bin/mocha test/api-test.js
```

</details>
