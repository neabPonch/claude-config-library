---
name: 8monkey-ai__hebo-platform__skill
source: https://github.com/8monkey-ai/hebo-platform/blob/9d7519a0675e32ddb482a4901ba7f92fba759bd7/.agents/skills/elysiajs/SKILL.md
repo: 8monkey-ai/hebo-platform
kind: skill
stars: 15
last_pushed: 2026-06-09T11:55:54Z
license: other
score: 9
domains: [backend-api, typescript]
tags: [elysiajs, bun, backend, api-design]
curated: 2026-06-15
curated_by: config-scout
---

# 8monkey-ai/hebo-platform — skill

**Why it's worth keeping:** It highlights critical edge cases like type loss during method chaining and explains how scope affects lifecycles to prevent context hallucinations. It also includes a specific recommended project structure.

**Summary:** Provides architectural patterns and technical nuances specifically for developing with the ElysiaJS framework.

**Source credibility:** From an AI-focused developer platform (8monkey-ai) specializing in conversational agents.

**Recency:** Current; reflects modern Bun/Elysia paradigms.

**Source:** [8monkey-ai/hebo-platform/.agents/skills/elysiajs/SKILL.md](https://github.com/8monkey-ai/hebo-platform/blob/9d7519a0675e32ddb482a4901ba7f92fba759bd7/.agents/skills/elysiajs/SKILL.md) · 15★

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
