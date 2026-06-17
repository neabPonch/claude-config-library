---
name: aolus-software__clean-elysia__skill
source: https://github.com/aolus-software/clean-elysia/blob/99ce05a08536636d615feef3ceeba62eb6e73ee5/.agents/skills/elysiajs/SKILL.md
repo: aolus-software/clean-elysia
kind: skill
stars: 20
last_pushed: 2026-06-04T08:50:00Z
license: mit
score: 9
domains: [backend-api, typescript]
tags: [elysiajs, bun, typebox, api-design]
curated: 2026-06-15
curated_by: config-scout
---

# aolus-software/clean-elysia — skill

**Why it's worth keeping:** It highlights critical TypeScript pitfalls like the 'method chaining' requirement for type inference and provides clear architectural rules for Controller/Service/Model separation.

**Summary:** Provides deep technical context for ElysiaJS, including type-safe validation patterns and a recommended domain-driven architecture.

**Source credibility:** High; comes from a specialized boilerplate repository with very recent maintenance.

**Recency:** Extremely current, utilizing modern Bun-centric patterns and llms.txt integration.

**Source:** [aolus-software/clean-elysia/.agents/skills/elysiajs/SKILL.md](https://github.com/aolus-software/clean-elysia/blob/99ce05a08536636d615feef3ceeba62eb6e73ee5/.agents/skills/elysiajs/SKILL.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: elysiajs
description: Create backend with ElysiaJS, a type-safe, high-performance framework.
---

# ElysiaJS Development Skill

Always consult [elysiajs.com/llms.txt](https://elysiajs.com/llms.txt) for code examples and latest API.

## Overview

ElysiaJS is a TypeScript framework for building Bun-first (but not limited to Bun) type-safe, high-performance backend servers. This skill provides comprehensive guidance for developing with Elysia, including routing, validation, authentication, plugins, integrations, and deployment.

## When to Use This Skill

Trigger this skill when the user asks to:

- Create or modify ElysiaJS routes, handlers, or servers
- Setup validation with TypeBox or other schema libraries (Zod, Valibot)
- Implement authentication (JWT, session-based, macros, guards)
- Add plugins (CORS, OpenAPI, Static files, JWT)
- Integrate with external services (Drizzle ORM, Better Auth, Next.js, Eden Treaty)
- Setup WebSocket endpoints for real-time features
- Create unit tests for Elysia instances
- Deploy Elysia servers to production

## Quick Start

Quick scaffold:

```bash
bun create elysia app
```

### Basic Server

```typescript
import { Elysia, t, status } f
```

</details>
