---
name: cammac-creator__ibanforge
source: https://github.com/cammac-creator/ibanforge/blob/92c7f4118c3595079794fa6dcf2c9c19a8a6ae96/CLAUDE.md
repo: cammac-creator/ibanforge
kind: claude-md
stars: 0
last_pushed: 2026-06-14T04:38:34Z
license: mit
score: 9
domains: [backend-api, fintech, mcp-servers]
tags: [typescript, sqlite, mcp, api]
curated: 2026-06-14
curated_by: config-scout
---

# cammac-creator/ibanforge — claude-md

**Why it's worth keeping:** It includes exact row counts/sources for SQLite databases and specific business-critical failure modes (x402 middleware) that prevent AI hallucinations regarding system readiness.

**Summary:** A highly dense technical specification that provides deep context on data structures, database contents, and operational constraints.

**Source credibility:** Recent individual project with specialized domain knowledge in fintech/MCP.

**Recency:** 

**Source:** [cammac-creator/ibanforge/CLAUDE.md](https://github.com/cammac-creator/ibanforge/blob/92c7f4118c3595079794fa6dcf2c9c19a8a6ae96/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# IBANforge

API de validation IBAN et lookup BIC/SWIFT avec micropaiements x402, interface MCP pour agents AI, données SEPA/VoP, classification émetteur (vIBAN detection), et indicateurs de risque compliance.

## Stack

- **Runtime** : Node.js 20+ / TypeScript
- **Framework** : Hono
- **Database** : SQLite (better-sqlite3) — `data/bic.sqlite` (121,399 BIC entries: 38,761 GLEIF + 81,642 SwiftCodes/MIT + 633 SIX + 201 EBA Step2 SCT + 142 Bundesbank + 19 NBP; plus 1,190 Swiss clearing entries SIX), `data/stats.sqlite`
- **Payments** : x402/hono (USDC micropayments)
- **AI Agents** : MCP SDK (Model Context Protocol)
- **Deploy** : Docker → Railway
- **Domain** : ibanforge.com

## Architecture

```
src/
  index.ts              # Entry point — Hono app + server
  types.ts              # Shared TypeScript types
  routes/
    iban-validate.ts    # POST /v1/iban/validate (single IBAN)
    iban-batch.ts       # POST /v1/iban/batch (up to 100)
    bic-lookup.ts       # GET /v1/bic/:code (BIC/SWIFT lookup)
    ch-clearing.ts      # GET /v1/ch/clearing/:iid (Swiss BC-Nummer lookup)
    health.ts           # GET /health
    stats.ts            # GET /stats
    landing.ts          # GET / (HTML
```

</details>
