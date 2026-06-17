---
name: plagesribeiro__svelte-hono-template
source: https://github.com/plagesribeiro/svelte-hono-template/blob/42cc39ea09416b8ad9cca7d599db84c4fc01733a/Claude.md
repo: plagesribeiro/svelte-hono-template
kind: claude-md
stars: 1
last_pushed: 2026-02-21T14:33:07Z
license: unknown
score: 9
domains: [fullstack, backend-api, monorepo]
tags: [sveltekit, hono, drizzle, turborepo, workflows]
curated: 2026-06-15
curated_by: config-scout
---

# plagesribeiro/svelte-hono-template — claude-md

**Why it's worth keeping:** The step-by-step 'Workflows' and specific naming convention tables provide perfect instruction for an AI agent to modify the codebase without constant prompting. It also explicitly details critical middleware ordering which prevents common logic errors.

**Summary:** A highly structured technical guide for a fullstack monorepo using SvelteKit, Hono, and Drizzle.

**Source credibility:** Low star count, but content depth suggests a professional, high-density production template.

**Recency:** Very current; uses SvelteKit 5 and modern toolchains like Biome.

**Source:** [plagesribeiro/svelte-hono-template/Claude.md](https://github.com/plagesribeiro/svelte-hono-template/blob/42cc39ea09416b8ad9cca7d599db84c4fc01733a/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Svelte-Hono Template

Turborepo monorepo: `apps/api` (Hono on CF Workers), `apps/web` (SvelteKit 5), `apps/db` (Drizzle ORM + Neon), `apps/shared` (Zod schemas & types). Auth via Clerk. See per-app CLAUDE.md for details.

## Architecture

- **Layered API**: Routes -> Services -> Repositories -> Database
- **Type-safe client**: Zod schemas in `shared` -> OpenAPI routes in `api` -> `ServerType` export -> `hcWithType` in `web`
- **Middleware order** (critical): `cors()` -> `clerkMiddleware()` -> [public/webhook routes] -> `authMiddleware()` -> [protected routes + db + services middleware]
- **Soft deletes**: All entities use `deletedAt` timestamp, repos always filter `isNull(deletedAt)`

## Naming Conventions

| What | Pattern | Example |
|------|---------|---------|
| Route files | `[name].route.ts` + `[name].index.ts` | `protected.route.ts` |
| DB tables | `dim_[entity]` | `dim_user`, `dim_organization` |
| Services | `[action]-[entity].ts` | `upsert-user-from-clerk.ts` |
| Repositories | `[entity].repo.ts` | `users.repo.ts` |
| Shared schemas | `[action][Entity][Request\|Response]Schema` | `getProtectedRouteRequestSchema` |
| Commits | Conventional commits | `feat:`, `fix:`, `ref
```

</details>
