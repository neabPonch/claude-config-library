---
name: openhab__openhab-cloud
source: https://github.com/openhab/openhab-cloud/blob/5c128d59a22a85fd3535e12f8a367756a5d3f475/CLAUDE.md
repo: openhab/openhab-cloud
kind: claude-md
stars: 307
last_pushed: 2026-05-29T21:28:17Z
license: epl-2.0
score: 9
domains: [backend-api, node-js, devops, testing]
tags: [typescript, express, docker, mongodb, integration-tests]
curated: 2026-06-14
curated_by: config-scout
---

# openhab/openhab-cloud — claude-md

**Why it's worth keeping:** It includes critical 'tribal knowledge' like DCO sign-off requirements and specific Docker orchestration steps that prevent workflow errors.

**Summary:** This file provides deep architectural context, specific data-flow logic, and precise command sequences for complex integration testing.

**Source credibility:** High; openHAB is a well-established, actively maintained open-source project.

**Recency:** Current; uses modern toolchains like tsx and Zod.

**Source:** [openhab/openhab-cloud/CLAUDE.md](https://github.com/openhab/openhab-cloud/blob/5c128d59a22a85fd3535e12f8a367756a5d3f475/CLAUDE.md) · 307★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

openHAB Cloud is a TypeScript/Node.js backend service for openHAB home automation. It provides secure remote access, push notifications, OAuth2 authorization, and cloud integrations for openHAB instances.

## Build & Development Commands

```bash
# Install dependencies
npm install

# Start the application (uses tsx for TypeScript)
npm start

# Build TypeScript to dist/
npm run build

# Type-check without emitting
npm run typecheck

# Run unit tests
npm test

# Run tests with coverage
npm run test:coverage

# Run integration tests (requires Docker)
npm run docker:test:up      # Start MongoDB, Redis
npm run docker:test:seed    # Seed test data
npm run test:integration    # Run integration tests
npm run docker:test:down    # Stop containers

# License headers
npm run license:check       # Check headers (dry run)
npm run license:update      # Add/update headers
```

## Configuration

Copy `config-production.json` to `config.json` and configure MongoDB, Redis, and system settings. The application reads configuration from `config.json` at startup.

##
```

</details>
