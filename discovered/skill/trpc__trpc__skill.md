---
name: trpc__trpc__skill
source: https://github.com/trpc/trpc/blob/3e0e9793eb7f8c4cfbe70a1dccb72f8d355e3c8b/packages/server/skills/trpc-router/SKILL.md
repo: trpc/trpc
kind: skill
stars: 40340
last_pushed: 2026-06-14T22:09:58Z
license: mit
score: 9
domains: [backend-api, typescript, web-development]
tags: [router, decision-tree, trpc, type-safe]
curated: 2026-06-15
curated_by: config-scout
---

# trpc/trpc — skill

**Why it's worth keeping:** The 'Master Router' pattern is highly transferable; it organizes vast documentation into logical task-based branches (Server/Host/Client) for efficient agent navigation.

**Summary:** A master 'router' skill that uses a decision tree to navigate the complex ecosystem of tRPC tasks.

**Source credibility:** Very high; based on the official, widely-used trpc repository with massive community backing.

**Recency:** Current; includes modern patterns like Next.js App Router and recent library versions.

**Source:** [trpc/trpc/packages/server/skills/trpc-router/SKILL.md](https://github.com/trpc/trpc/blob/3e0e9793eb7f8c4cfbe70a1dccb72f8d355e3c8b/packages/server/skills/trpc-router/SKILL.md) · 40340★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: trpc-router
description: >
  Entry point for all tRPC skills. Decision tree routing by task: initTRPC.create(),
  t.router(), t.procedure, createTRPCClient, adapters, subscriptions, React Query,
  Next.js, links, middleware, validators, error handling, caching, FormData.
type: core
library: trpc
library_version: '11.16.0'
requires: []
sources:
  - 'trpc/trpc:www/docs/main/introduction.mdx'
  - 'trpc/trpc:www/docs/main/quickstart.mdx'
---

# tRPC -- Skill Router

## Decision Tree

### What are you trying to do?

#### Define a tRPC backend (server)

- **Initialize tRPC, define routers, procedures, context, export AppRouter**
  -> Load skill: `server-setup`

- **Add middleware (.use), auth guards, logging, base procedures**
  -> Load skill: `middlewares`

- **Add input/output validation with Zod or other libraries**
  -> Load skill: `validators`

- **Throw typed errors, format errors for clients, global error handling**
  -> Load skill: `error-handling`

- **Call procedures from server code, write integration tests**
  -> Load skill: `server-side-calls`

- **Set Cache-Control headers on query responses (CDN, browser caching)**
  -> Load skill: `caching`

- **Accept FormData,
```

</details>
