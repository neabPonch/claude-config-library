---
name: mattmck__swatchwatch
source: https://github.com/mattmck/swatchwatch/blob/016ee24234616939df78f4bd4d7a5e78b0ebfc20/CLAUDE.md
repo: mattmck/swatchwatch
kind: claude-md
stars: 0
last_pushed: 2026-06-10T19:36:36Z
license: unknown
score: 9
domains: [fullstack, monorepo, cloud-infrastructure]
tags: [azure, typescript, nextjs, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# mattmck/swatchwatch — claude-md

**Why it's worth keeping:** Includes specific 'tribal knowledge' like exact pattern registrations for Azure Functions v4, path aliases, and color utility logic. The 'Known State & TODOs' section is a masterclass in preventing AI hallucination regarding feature completeness.

**Summary:** Maps a complex full-stack monorepo involving Next.js, Expo, and Azure Functions with clear data flow and deployment targets. It provides high-density technical context that allows an agent to navigate the entire stack.

**Source credibility:** Low public visibility (0 stars), but the technical depth suggests a sophisticated real-world engineering project.

**Recency:** Highly current; utilizes modern versions of Tailwind (v4) and Next.js App Router.

**Source:** [mattmck/swatchwatch/CLAUDE.md](https://github.com/mattmck/swatchwatch/blob/016ee24234616939df78f4bd4d7a5e78b0ebfc20/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SwatchWatch — Agent Instructions

## Architecture Overview

Smart nail polish collection manager. **npm workspaces monorepo** with three deployable targets and a shared types package:

```
apps/web          → Next.js 16 (App Router) + Tailwind v4 + shadcn/ui → Azure Static Web App
apps/mobile       → Expo / React Native (SDK 54, RN 0.81)
packages/functions → Azure Functions v4 (Node 20, TS)    → Azure Linux Function App
packages/shared    → Shared TypeScript types (polish, user, voice)
infrastructure/    → Terraform (azurerm ~3.100) for all Azure resources
```

**Data flow:** Clients → Azure Functions REST API (`/api/polishes`, `/api/auth/*`, `/api/voice`) → Azure Database for PostgreSQL Flexible Server (schema in `docs/schema.sql`). Voice input goes through Azure Speech Services → Azure OpenAI for parsing polish details from transcriptions. Full canonical schema uses `pg_trgm` for fuzzy shade matching and `pgvector` for swatch similarity/dupe search.

**Auth:** Azure AD B2C (provisioned outside Terraform via portal). Functions read `AZURE_AD_B2C_TENANT` and `AZURE_AD_B2C_CLIENT_ID` from environment. Token validation is JWT-based via the `/api/auth/validate` endpoint.

## Dev Com
```

</details>
