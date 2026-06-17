---
name: OregonStateHackathonClub__website
source: https://github.com/OregonStateHackathonClub/website/blob/7eb0ef460beba54a3e95b99090c6f806857a361d/claude.md
repo: OregonStateHackathonClub/website
kind: claude-md
stars: 8
last_pushed: 2026-05-07T23:31:52Z
license: unknown
score: 8
domains: [web-frontend, fullstack, monorepo]
tags: [monorepo, nextjs, architectural-rules]
curated: 2026-06-14
curated_by: config-scout
---

# OregonStateHackathonClub/website — claude-md

**Why it's worth keeping:** Uses 'gold standard' references for UI/UX consistency and provides high-value negative constraints to prevent over-engineering and scope creep.

**Summary:** Provides strict architectural constraints for a Next.js monorepo, covering server actions, Prisma patterns, and routing logic.

**Source credibility:** A small but highly organized student organization monorepo with clear engineering standards.

**Recency:** Very current; aligns with modern Next.js App Router patterns.

**Source:** [OregonStateHackathonClub/website/claude.md](https://github.com/OregonStateHackathonClub/website/blob/7eb0ef460beba54a3e95b99090c6f806857a361d/claude.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# BeaverHacks Monorepo

Hackathon management monorepo for Oregon State University's Hackathon Club.

## Apps

- `beaverhacks` - Main site, applications (port 3000)
- `judge` - Judging & submissions (port 3002)
- `admin` - Admin dashboard (port 3004)
- `shop` - Merchandise (port 3001)
- `career` - Sponsorships (port 3003)

## Code Conventions

### General

- Server components by default, `"use client"` only when needed
- Use `@repo/ui`, `@repo/auth`, `@repo/database` for shared code
- Reference implementation: **apps/admin** is the gold standard

### Server Actions

- Use server actions for all mutations, not API routes
- Exception: Binary file downloads, external service redirects (Stripe)
- Every action starts with auth check (e.g., `await requireAdmin()`)
- Return `{ success: true }` or `{ success: false, error: string }`
- Call `revalidatePath()` after mutations

### Prisma

- Always use `select` to limit fields returned
- Use `_count` for statistics instead of fetching full records
- Parallel queries with `Promise.all()` where possible

### Route Protection

- Use `(authenticated)` route group with auth check in layout
- Redirect unauthenticated users to login with `callbackURL
```

</details>
