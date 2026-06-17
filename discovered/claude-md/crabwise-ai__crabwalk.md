---
name: crabwise-ai__crabwalk
source: https://github.com/crabwise-ai/crabwalk/blob/ea99ca93fd36b4aa2991a0b1401974bb0e881c15/CLAUDE.md
repo: crabwise-ai/crabwalk
kind: claude-md
stars: 878
last_pushed: 2026-02-19T18:35:52Z
license: mit
score: 8
domains: [web-frontend, fullstack-development, real-time-data]
tags: [tanstack, trpc, react-19, tailwindcss-v4]
curated: 2026-06-15
curated_by: config-scout
---

# crabwise-ai/crabwalk — claude-md

**Why it's worth keeping:** It defines specific implementation patterns (tRPC and TanStack DB) rather than just listing files, which tells Claude *how* to extend the code. The explanation of the real-time data flow through the OpenClaw gateway is crucial for understanding the app's unique logic.

**Summary:** Provides structured architectural context for a modern TanStack-based full-stack application.

**Source credibility:** The project is well-regarded in its niche with nearly 900 stars.

**Recency:** 

**Source:** [crabwise-ai/crabwalk/CLAUDE.md](https://github.com/crabwise-ai/crabwalk/blob/ea99ca93fd36b4aa2991a0b1401974bb0e881c15/CLAUDE.md) · 878★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # start dev server on port 3000
npm run build    # production build
npm start        # run production server (dist/server/server.js)
```

## Architecture

Full-stack React app using TanStack Start (file-based routing, SSR).

**Stack:**
- TanStack Start + Router (file-based routing)
- tRPC (API layer w/ superjson transformer)
- TanStack Query (data fetching)
- TanStack DB (client-side reactive collections)
- Tailwind CSS v4
- React 19

**Key paths:**
- `src/routes/` - file-based routes, auto-generates `routeTree.gen`
- `src/routes/api/trpc.$.ts` - tRPC catch-all API handler
- `src/integrations/trpc/router.ts` - tRPC router definition (`appRouter`)
- `src/integrations/trpc/client.ts` - tRPC client
- `src/integrations/query/provider.tsx` - React Query provider
- `src/router.tsx` - TanStack Router config

**Path alias:** `~/` maps to `src/`

**tRPC pattern:** Add procedures to `appRouter` in `router.ts`, import `trpc` from `client.ts` to call.

**TanStack DB pattern:** Create collections, use `useLiveQuery()` for reactive reads, `cre
```

</details>
