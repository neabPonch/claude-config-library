---
name: saitadikonda99__dodge.ai
source: https://github.com/saitadikonda99/dodge.ai/blob/e3d26298902c29c33e5815e0c6d2b9646c7edc5c/claude.md
repo: saitadikonda99/dodge.ai
kind: claude-md
stars: 0
last_pushed: 2026-03-25T02:04:05Z
license: mit
score: 7
domains: [web-fullstack, software-architecture]
tags: [layering, logging, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# saitadikonda99/dodge.ai — claude-md

**Why it's worth keeping:** The rigid layer-order constraints prevent logic leakage, while the mandatory session log creates a highly effective audit trail of AI decisions and file changes.

**Summary:** Enforces strict architectural layering for a Node/Next.js stack and mandates proactive session logging for agent accountability.

**Source credibility:** Low; it is from an unstarred repository with minimal social proof.

**Recency:** High; the logging mechanism is specifically useful for managing long-context agentic workflows like Claude Code.

**Source:** [saitadikonda99/dodge.ai/claude.md](https://github.com/saitadikonda99/dodge.ai/blob/e3d26298902c29c33e5815e0c6d2b9646c7edc5c/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Architecture Rules (STRICT)

### Backend (node-server)
Layer order: controller → service → repository → db
- Controllers: HTTP request/response only. No business logic. No DB calls.
- Services: Business logic only. Calls repositories and LLM. No Express imports.
- Repositories: DB queries only. mysql2/promise. No business logic.
- Domain: Pure TypeScript interfaces. Zero imports from other layers.
- Never use process.env directly — always use config/env.ts
- Never throw raw Error — always throw AppError from utils/errors.ts

### Frontend (nextjs-client)
- Components: UI only. No API calls. No business logic.
- Hooks: All data fetching and state logic.
- lib/api.ts: Only place for backend API calls. Never call fetch in components.
- types/: All TypeScript interfaces. No imports from other layers.
- Never use process.env directly — use lib/constants.ts
- Never default export except page.tsx and layout.tsx
- Always use Tailwind CSS — no inline styles
- All graph components must have 'use client' directive

### Both
- Never use `any` types
- Always use async/await, never .then()
- Always use named exports

## Session Logging (MANDATORY)

After EVERY prompt, append to session-logs/cl
```

</details>
