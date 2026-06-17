---
name: orval-labs__orval__skill
source: https://github.com/orval-labs/orval/blob/89e0de8d5d295fd0b1c5ceb8d6801252f42aa82f/skills/orval/SKILL.md
repo: orval-labs/orval
kind: skill
stars: 6124
last_pushed: 2026-06-14T23:08:59Z
license: mit
score: 9
domains: [web-frontend, api-client-generation, typescript]
tags: [openapi, codegen, typescript, react-query]
curated: 2026-06-15
curated_by: config-scout
---

# orval-labs/orval — skill

**Why it's worth keeping:** The decision matrices (Client Selection Guide) provide clear, actionable logic that an agent can use to recommend specific configurations based on user requirements.

**Summary:** A highly detailed specification for the Orval OpenAPI generator, covering client selection, mode selection, and output configuration.

**Source credibility:** High: highly popular open-source tool (6k+ stars) with recent maintenance.

**Recency:** Current: includes modern framework support like TanStack Query and MCP servers.

**Source:** [orval-labs/orval/skills/orval/SKILL.md](https://github.com/orval-labs/orval/blob/89e0de8d5d295fd0b1c5ceb8d6801252f42aa82f/skills/orval/SKILL.md) · 6124★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: orval
description: Generate type-safe API clients, TanStack Query/SWR hooks, Zod schemas, MSW mocks, Hono server handlers, MCP servers, and SolidStart actions from OpenAPI specs using Orval. Covers all clients (React/Vue/Svelte/Solid/Angular Query, Fetch, Axios), custom HTTP mutators, authentication patterns, NDJSON streaming, programmatic API, and advanced configuration.
---

# Orval - OpenAPI to TypeScript Code Generator

Orval generates type-safe TypeScript clients, hooks, schemas, mocks, and server handlers from OpenAPI v3/Swagger v2 specifications.

## Quick Start

### Installation

```bash
npm install orval -D
# or yarn add orval -D
# or pnpm add orval -D
# or bun add orval -D
```

### Minimal Configuration

```ts
import { defineConfig } from 'orval';

export default defineConfig({
  petstore: {
    input: {
      target: './petstore.yaml',
    },
    output: {
      target: './src/api/petstore.ts',
      schemas: './src/api/model',
      client: 'react-query',
    },
  },
});
```

### Run

```bash
npx orval
npx orval --config ./orval.config.ts
npx orval --project petstore
npx orval --watch
```

## Choosing Your Setup

### Client Selection Guide

| Use Case
```

</details>
