---
name: onecli__onecli
source: https://github.com/onecli/onecli/blob/622cb267c61e4769ed7bfd70499ad45bf816ea63/CLAUDE.md
repo: onecli/onecli
kind: claude-md
stars: 2375
last_pushed: 2026-06-14T11:06:35Z
license: apache-2.0
score: 9
domains: [web-frontend, backend-api, fullstack]
tags: [nextjs, typescript, prisma, aws, shadcn]
curated: 2026-06-15
curated_by: config-scout
---

# onecli/onecli — claude-md

**Why it's worth keeping:** It includes concrete code patterns for specialized business logic (audit logging) and explicit constraints on component structure and prop typing to maintain UI consistency.

**Summary:** A highly structured technical manual for a full-stack Next.js and AWS application that provides strict architectural guardrails.

**Source credibility:** High; comes from an active, highly-starred open-source project.

**Recency:** Very current, utilizing modern Next.js App Router and shadcn/ui conventions.

**Source:** [onecli/onecli/CLAUDE.md](https://github.com/onecli/onecli/blob/622cb267c61e4769ed7bfd70499ad45bf816ea63/CLAUDE.md) · 2375★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OneCLI

Cloud backend for OneCLI — manages authentication, integrations, and permissions for the OneCLI agent gateway.

## Commands

```bash
pnpm dev          # Start development
pnpm build        # Build all
pnpm check        # Lint + types + format
pnpm fix          # Auto-fix lint + format
pnpm db:generate  # Generate Prisma client
pnpm db:migrate   # Run migrations (dev)
pnpm db:studio    # Open Prisma Studio
```

## Structure

```
apps/web/         # Next.js 16 app (App Router)
packages/db/      # Prisma ORM + migrations
packages/infra/   # AWS CDK infrastructure
packages/ui/      # Shared components (shadcn/ui)
packages/eslint-config/
packages/typescript-config/
```

## Environment Variables

- `DATABASE_URL`: PostgreSQL connection string
- `NEXT_PUBLIC_COGNITO_*`: AWS Cognito config (injected at build time in CI)
- `STRIPE_SECRET_KEY`, `GOOGLE_CLIENT_ID`, `GOOGLE_CLIENT_SECRET`: Third-party credentials

## Code Style

- **Use strong typing** - leverage types from external packages; avoid `any` and type assertions
- Prefer named exports over default exports (except Next.js pages/layouts where required)
- Use `@onecli/ui/*` for shared UI imports, `@/` for app-local imports
-
```

</details>
