---
name: getclawe__clawe
source: https://github.com/getclawe/clawe/blob/3214feda034b8a4924b4fb11c17c5129f099658c/CLAUDE.md
repo: getclawe/clawe
kind: claude-md
stars: 729
last_pushed: 2026-02-23T13:58:20Z
license: agpl-3.0
score: 8
domains: [web-frontend, fullstack, monorepo]
tags: [nextjs, convex, shadcn, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# getclawe/clawe — claude-md

**Why it's worth keeping:** Includes highly effective 'Allowed vs Not Allowed' guardrails for shadcn/ui to prevent component destruction, and provides strict type-safety mandates that reduce AI errors.

**Summary:** Provides comprehensive architectural and workflow context for a Next.js/Convex monorepo, including clear command lists and data layer usage patterns.

**Source credibility:** High; 729 stars indicates a significant and active open-source project.

**Recency:** Highly current, reflecting modern full-stack development practices from the last few months.

**Source:** [getclawe/clawe/CLAUDE.md](https://github.com/getclawe/clawe/blob/3214feda034b8a4924b4fb11c17c5129f099658c/CLAUDE.md) · 729★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Clawe

Open-source orchestration layer for OpenClaw - makes multi-agent AI systems accessible to everyone.

## Commands

```bash
pnpm dev          # Start development
pnpm convex:dev   # Start Convex dev server
pnpm build        # Build all
pnpm check        # Lint + types + format
pnpm fix          # Auto-fix lint + format
```

## Structure

```
apps/web/                  # Next.js 16 app (App Router)
  └── src/app/api/         # API routes (health, webhooks, integrations)
packages/backend/          # Convex backend (schema, queries, mutations)
  └── convex/              # Convex functions and schema
packages/shared/           # Shared DTOs (Agent, Task, Message types)
packages/ui/               # Shared components (shadcn/ui)
packages/eslint-config/
packages/typescript-config/
```

## Data Layer

**Convex** - Real-time backend for core data (agents, tasks, messages):

```tsx
"use client";
import { useQuery, useMutation } from "convex/react";
import { api } from "@clawe/backend";

const agents = useQuery(api.agents.list);
const createAgent = useMutation(api.agents.create);
```

**Next.js API Routes** - For webhooks and external integrations (`/api/*`):

```typescript
// app/api/
```

</details>
