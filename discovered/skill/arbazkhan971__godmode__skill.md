---
name: arbazkhan971__godmode__skill
source: https://github.com/arbazkhan971/godmode/blob/8dceddc656f280c791b362a5f1f21fd6ef3d0ab8/skills/nextjs/SKILL.md
repo: arbazkhan971/godmode
kind: skill
stars: 22
last_pushed: 2026-04-25T21:47:23Z
license: mit
score: 8
domains: [web-frontend, nextjs]
tags: [nextjs, app-router, performance, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# arbazkhan971/godmode — skill

**Why it's worth keeping:** It includes proactive discovery shell commands (cat, ls, grep) to sense project state and enforces high-value 'Hard Rules' regarding component boundaries and rendering strategies.

**Summary:** An expert-level Next.js workflow that uses environmental sensing commands and strict architectural constraints to guide an autonomous agent.

**Source credibility:** A specialized, high-effort toolset with specific focus on agentic optimization.

**Recency:** Highly current, explicitly mentioning Next.js 15+ and the App Router architecture.

**Source:** [arbazkhan971/godmode/skills/nextjs/SKILL.md](https://github.com/arbazkhan971/godmode/blob/8dceddc656f280c791b362a5f1f21fd6ef3d0ab8/skills/nextjs/SKILL.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nextjs
description: Next.js mastery -- App Router, Server Components,
  data fetching, rendering strategies, optimization.
---

## Activate When
- `/godmode:nextjs`, "Next.js", "App Router"
- "Server Components", "server actions", "ISR"
- "SSG", "SSR", "next/image", "middleware"
- "nextjs page", "Next.js page", "nextjs dashboard"

## Workflow

### 1. Project Assessment
```bash
cat next.config.* 2>/dev/null
ls app/ pages/ 2>/dev/null
grep "next" package.json 2>/dev/null
```
```
Router: App Router | Pages Router | Migration
Version: 13 | 14 | 15+
Rendering: mostly static | mostly dynamic | mixed
Auth: NextAuth | Clerk | Supabase Auth | custom
Deploy: Vercel | self-hosted | Docker
```

### 2. App Router Architecture
```
app/
  layout.tsx          # Root (metadata, providers)
  loading.tsx / error.tsx / not-found.tsx
  (marketing)/        # Route group (no URL segment)
    page.tsx, about/, pricing/
  (app)/              # Authenticated app group
    layout.tsx (sidebar, nav)
    dashboard/ (page, loading, error)
    [workspace]/ (dynamic, [...slug]/)
  api/ (route handlers)
```
Route groups `(name)` organize without URL impact.
Every segment: layout, loading, error optional.
```

</details>
