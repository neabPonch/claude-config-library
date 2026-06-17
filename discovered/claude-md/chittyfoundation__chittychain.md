---
name: chittyfoundation__chittychain
source: https://github.com/chittyfoundation/chittychain/blob/2994f31b44c4488b90c5f59a94a97af2789156f8/CLAUDE.md
repo: chittyfoundation/chittychain
kind: claude-md
stars: 0
last_pushed: 2026-04-25T02:00:53Z
license: mit
score: 8
domains: [blockchain, full-stack, api]
tags: [architecture-heavy, ecosystem-context, smart-contracts]
curated: 2026-06-17
curated_by: config-scout
---

# chittyfoundation/chittychain — claude-md

**Why it's worth keeping:** Includes conceptual architectural models (Dual Immutability) and a dependency map of related services, providing crucial context for system-wide understanding beyond just file paths.

**Summary:** A comprehensive technical blueprint covering full-stack architecture, blockchain integration, and ecosystem relationships.

**Source credibility:** Low social proof/stars but highly detailed documentation suggests an active, specialized project.

**Recency:** Current; utilizes modern stacks like Vite, Drizzle, and Neon.

**Source:** [chittyfoundation/chittychain/CLAUDE.md](https://github.com/chittyfoundation/chittychain/blob/2994f31b44c4488b90c5f59a94a97af2789156f8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

ChittyChain is the on-chain anchor layer for the ChittyOS ecosystem. It provides immutable finality for governance decisions, attribution traces, and evidence records. While ChittyLedger is the fast off-chain database layer, ChittyChain is the permanent on-chain record of truth. Full-stack application with Express backend, React frontend, and Solidity smart contracts.

**Repo:** `CHITTYFOUNDATION/chittychain`
**Deploy:** Docker/Kubernetes, Cloudflare Workers (edge)
**Stack:** Express + TypeScript (backend), React + Vite + Tailwind (frontend), Drizzle ORM, Neon PostgreSQL, Solidity/OpenZeppelin, ethers.js, Socket.IO
**Canonical URI:** `chittycanon://core/services/chitty-chain` | Tier 0

## Common Commands

```bash
npm run dev              # Start Express dev server (tsx, NODE_ENV=development)
npm run build            # Build frontend (Vite) + bundle server (esbuild)
npm start                # Start production server (node dist/index.js)
npm run check            # TypeScript type-check
npm run db:push          # Push Drizzle schema to database
npm test                 # Run vitest test suite
npm run test:run         # Run tests once
npm run test:secu
```

</details>
