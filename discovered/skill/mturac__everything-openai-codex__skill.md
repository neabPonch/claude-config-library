---
name: mturac__everything-openai-codex__skill
source: https://github.com/mturac/everything-openai-codex/blob/b5057da5f42ed6b12cd3a59e89af0ccd12cff7c2/skills/backend-patterns/SKILL.md
repo: mturac/everything-openai-codex
kind: skill
stars: 78
last_pushed: 2026-06-15T12:56:01Z
license: mit
score: 9
domains: [backend-api, database-optimization, web-development]
tags: [typescript, nodejs, architecture, patterns]
curated: 2026-06-17
curated_by: config-scout
---

# mturac/everything-openai-codex — skill

**Why it's worth keeping:** Uses high-signal 'PASS/FAIL' comparative examples; provides specific, actionable strategies for N+1 prevention and transaction management that are highly transferable to any agentic workflow.

**Summary:** A comprehensive reference for backend architecture patterns including Repository/Service layers, API design, and database optimization.

**Source credibility:** Solid community interest with 78 stars and very recent activity.

**Recency:** Extremely current, focusing on modern stacks like Next.js, Supabase, and TypeScript.

**Source:** [mturac/everything-openai-codex/skills/backend-patterns/SKILL.md](https://github.com/mturac/everything-openai-codex/blob/b5057da5f42ed6b12cd3a59e89af0ccd12cff7c2/skills/backend-patterns/SKILL.md) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: backend-patterns
description: Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes.
origin: ecc
---

# Backend Development Patterns

Backend architecture patterns and best practices for scalable server-side applications.

## When to Activate

- Designing REST or GraphQL API endpoints
- Implementing repository, service, or controller layers
- Optimizing database queries (N+1, indexing, connection pooling)
- Adding caching (Redis, in-memory, HTTP cache headers)
- Setting up background jobs or async processing
- Structuring error handling and validation for APIs
- Building middleware (auth, logging, rate limiting)

## API Design Patterns

### RESTful API Structure

```typescript
// PASS: Resource-based URLs
GET    /api/markets                 # List resources
GET    /api/markets/:id             # Get single resource
POST   /api/markets                 # Create resource
PUT    /api/markets/:id             # Replace resource
PATCH  /api/markets/:id             # Update resource
DELETE /api/markets/:id             # Delete resource

// PASS: Query parameters for filtering, sorting, paginati
```

</details>
