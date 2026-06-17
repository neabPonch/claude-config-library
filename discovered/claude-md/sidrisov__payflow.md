---
name: sidrisov__payflow
source: https://github.com/sidrisov/payflow/blob/b37681f8e9d0b34b9eafd79ef4fb4a7eb337c020/CLAUDE.md
repo: sidrisov/payflow
kind: claude-md
stars: 28
last_pushed: 2026-01-25T13:04:59Z
license: gpl-3.0
score: 9
domains: [monorepo, web3, fullstack]
tags: [npm-workspaces, spring-boot, react, typescript, blockchain]
curated: 2026-06-15
curated_by: config-scout
---

# sidrisov/payflow — claude-md

**Why it's worth keeping:** Uses explicit 'npm --workspace' and Gradle patterns to eliminate command guesswork in a monorepo; provides architectural layering rules that ensure LLM code generation matches existing patterns.

**Summary:** A highly detailed blueprint for a complex multi-language monorepo containing React, NestJS, and Java services. It maps the entire project landscape including specific workspace commands.

**Source credibility:** Specialized Web3 project with high-density technical documentation.

**Recency:** Highly current, utilizing modern tech stacks like React 19 and Java 21.

**Source:** [sidrisov/payflow/CLAUDE.md](https://github.com/sidrisov/payflow/blob/b37681f8e9d0b34b9eafd79ef4fb4a7eb337c020/CLAUDE.md) · 28★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Payflow is an onchain social payments ecosystem built on Web3 technologies, focused on Farcaster integration. It's a monorepo containing multiple frontend apps, backend services, and shared packages for cross-chain payment functionality across Base, Optimism, Arbitrum, Zora, Mode, Degen L3, Worldchain, and Polygon.

## Monorepo Structure

This is an npm workspaces monorepo with the following components:

### Core Applications

**`app/`** - Main Payflow PWA (Progressive Web App)
- React 19 + TypeScript + Vite
- Material UI v7 for components
- Privy for authentication, Wagmi for wallet interactions
- SSR support with custom Express server
- Entry points: `src/entry-client.tsx` (CSR), `src/entry-server.tsx` (SSR), `server.js` (Express)

**`home/`** - Marketing/landing page
- React 19 + TypeScript + Vite
- Lighter dependencies, focused on presentation

### Services

**`services/payflow-service/`** - Backend API (Spring Boot + Java 21 + Gradle)
- REST API and GraphQL endpoints
- JPA with MySQL/H2 database
- Redis/Caffeine caching layers
- Flyway migra
```

</details>
