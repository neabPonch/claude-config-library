---
name: vwh__temp-mail
source: https://github.com/vwh/temp-mail/blob/720bc5b1b61aab8901d670cfca07b79bbe4bb189/CLAUDE.md
repo: vwh/temp-mail
kind: claude-md
stars: 111
last_pushed: 2026-04-06T04:54:44Z
license: mit
score: 9
domains: [backend-api, edge-computing, serverless]
tags: [cloudflare-workers, typescript, bun, hono]
curated: 2026-06-15
curated_by: config-scout
---

# vwh/temp-mail — claude-md

**Why it's worth keeping:** The inclusion of specific 'Architecture Patterns' prevents structural drift, while the detailed directory tree and Biome style guidelines ensure code consistency during generation.

**Summary:** A comprehensive technical blueprint that covers architecture, command execution, and environmental setup for a Cloudflare-native application.

**Source credibility:** High; a well-documented, starred repository with up-to-date maintenance history.

**Recency:** Current; uses modern toolchains like Bun and Biome that are highly compatible with Claude Code's capabilities.

**Source:** [vwh/temp-mail/CLAUDE.md](https://github.com/vwh/temp-mail/blob/720bc5b1b61aab8901d670cfca07b79bbe4bb189/CLAUDE.md) · 111★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Temp Mail Worker - Claude Code Instructions

This repository is a **Cloudflare Workers-based temporary email service** that provides disposable email addresses with attachment support. The service receives emails via Cloudflare Email Routing, stores them in D1 database, and provides REST API endpoints for managing emails and attachments.

## Project Overview

- **Type**: Cloudflare Worker + Hono Framework
- **Purpose**: Temporary email service with attachment support
- **Live API**: https://api.barid.site
- **Web Client**: https://web.barid.site
- **Runtime**: Cloudflare Workers (Edge Computing)
- **Package Manager**: Bun

## Technology Stack

### Core Technologies
- **Runtime**: Cloudflare Workers (Edge Computing)
- **Framework**: Hono.js (Lightweight web framework)
- **Language**: TypeScript (ESNext target)
- **Package Manager**: Bun

### Key Dependencies
- **@hono/zod-openapi**: OpenAPI documentation generation
- **@hono/zod-validator**: Request validation with Zod
- **zod**: Schema validation
- **postal-mime**: Email parsing
- **html-to-text**: HTML content conversion
- **@paralleldrive/cuid2**: Unique ID generation

### Development Tools
- **Biome**: Code formatting and lint
```

</details>
