---
name: jralvarenga__better-translate__skill
source: https://github.com/jralvarenga/better-translate/blob/28b1300f40d3590bc4f16df25aab5aac95f8f6f4/.agents/skills/elysiajs/SKILL.md
repo: jralvarenga/better-translate
kind: skill
stars: 23
last_pushed: 2026-06-06T16:25:17Z
license: mit
score: 9
domains: [backend-api, typescript]
tags: [elysiajs, bun, type-safety, server-side]
curated: 2026-06-15
curated_by: config-scout
---

# jralvarenga/better-translate — skill

**Why it's worth keeping:** It documents critical framework 'gotchas' like the necessity of method chaining for type retention and explains complex lifecycle scoping/encapsulation. The instruction to consult a specific llms.txt URL is an elite pattern for maintaining up-to-date agent knowledge.

**Summary:** A highly specialized guide for ElysiaJS that covers everything from basic routing to advanced type-safe validation and architectural patterns.

**Source credibility:** The content shows high manual curation, likely written by a practitioner rather than generated via template.

**Recency:** Very current; includes modern Bun-first ecosystem patterns and latest TypeScript integration techniques.

**Source:** [jralvarenga/better-translate/.agents/skills/elysiajs/SKILL.md](https://github.com/jralvarenga/better-translate/blob/28b1300f40d3590bc4f16df25aab5aac95f8f6f4/.agents/skills/elysiajs/SKILL.md) · 23★

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
import { Elysia, t, status } from
```

</details>
