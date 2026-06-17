---
name: hicommonwealth__commonwealth
source: https://github.com/hicommonwealth/commonwealth/blob/fca71cca527b490e3f3ad955044a0506139d0330/CLAUDE.md
repo: hicommonwealth/commonwealth
kind: claude-md
stars: 90
last_pushed: 2026-05-21T18:50:40Z
license: gpl-3.0
score: 9
domains: [fullstack, monorepo, blockchain]
tags: [typescript, architecture-map, cli-reference]
curated: 2026-06-15
curated_by: config-scout
---

# hicommonwealth/commonwealth — claude-md

**Why it's worth keeping:** It uses categorized CLI blocks for easy reference and provides functional directory mapping that explains the purpose of folders rather than just their location.

**Summary:** A comprehensive guide for a complex TypeScript monorepo covering setup, command categories, and system architecture.

**Source credibility:** High-quality open source project with significant stars and recent activity.

**Recency:** Extremely current, utilizing Node 22 and pnpm 9.

**Source:** [hicommonwealth/commonwealth/CLAUDE.md](https://github.com/hicommonwealth/commonwealth/blob/fca71cca527b490e3f3ad955044a0506139d0330/CLAUDE.md) · 90★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

Commonwealth is a full-stack TypeScript monorepo for a multi-tenant blockchain community platform. The application supports multiple blockchains (EVM, Cosmos, Solana) with on-chain governance, real-time notifications, and community engagement features.

## Prerequisites

- Node.js 22.x
- pnpm 9.14.2
- Docker (for PostgreSQL, RabbitMQ, Redis)
- PostgreSQL client (psql)

## Setup

```bash
# Install dependencies
pnpm install

# Set up environment variables
cp .env.example .env

# Start external services (PostgreSQL, Redis, RabbitMQ)
docker-compose up -d

# Run database migrations
pnpm migrate-db

# Start the application (API + frontend)
pnpm start
```

The API server runs on http://localhost:3000 (health check at /api/health) and the client on http://localhost:8080.

## Common Commands

### Development

```bash
# Start API server and frontend (most common for local dev)
pnpm start

# Start only the API server
pnpm -F commonwealth start-api

# Start only the frontend
pnpm -F commonwealth start-frontend

# Start all microservices (requires RabbitMQ
```

</details>
