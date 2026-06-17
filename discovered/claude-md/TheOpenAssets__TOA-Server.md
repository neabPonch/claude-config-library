---
name: TheOpenAssets__TOA-Server
source: https://github.com/TheOpenAssets/TOA-Server/blob/82053ac3f687f39555a393d89c774dc29cbe2d79/claude.md
repo: TheOpenAssets/TOA-Server
kind: claude-md
stars: 0
last_pushed: 2026-04-15T19:48:05Z
license: unknown
score: 8
domains: [backend-api, blockchain]
tags: [monorepo, context-driven, nest-js, architecture]
curated: 2026-06-17
curated_by: config-scout
---

# TheOpenAssets/TOA-Server — claude-md

**Why it's worth keeping:** The mandatory use of local 'context.md' files in every module prevents knowledge drift; the 'Rule of Plans' encourages high-level reasoning over premature code generation.

**Summary:** Establishes strict architectural boundaries for a complex NestJS monorepo and introduces a unique 'context.md' pattern.

**Source credibility:** Low social proof (0 stars), but demonstrates sophisticated architectural planning for a production-grade blockchain backend.

**Recency:** Very recent (2 months ago), highly relevant to agentic workflow patterns.

**Source:** [TheOpenAssets/TOA-Server/claude.md](https://github.com/TheOpenAssets/TOA-Server/blob/82053ac3f687f39555a393d89c774dc29cbe2d79/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Open Assets Backend

## Project Summary

Open Assets is a Real-World Asset (RWA) tokenization platform that enables the full lifecycle of bringing real-world assets on-chain — from originator onboarding and KYC verification, through asset attestation and token deployment, to primary marketplace listing (static pricing and auctions), secondary P2P trading, yield distribution, and settlement.

The platform is built as a NestJS monorepo with three packages: a backend REST API, Solidity smart contracts, and shared TypeScript types. The backend orchestrates 17 domain modules — Auth, Admin, Assets, Blockchain, KYC, Marketplace, Secondary Market, Yield, Leverage, Solvency, Partners, Notifications, Announcements, Changelog, Compliance Engine, Faucet, and Typeform — all communicating through NestJS dependency injection with MongoDB for persistence, Redis/BullMQ for async event processing, and a global Blockchain module that handles all on-chain interactions.

The on-chain layer consists of 17 deployed smart contracts on Mantle Sepolia covering asset attestation (AttestationRegistry), identity verification (IdentityRegistry, OAID), token lifecycle (TokenFactory, RWAToken, Priva
```

</details>
