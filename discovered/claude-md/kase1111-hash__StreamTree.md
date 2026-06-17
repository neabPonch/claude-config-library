---
name: kase1111-hash__StreamTree
source: https://github.com/kase1111-hash/StreamTree/blob/7d6d83c30d9bc7662e79bcc18ef50c2c8f510a44/claude.md
repo: kase1111-hash/StreamTree
kind: claude-md
stars: 1
last_pushed: 2026-02-23T02:22:05Z
license: mit
score: 8
domains: [full-stack, monorepo, web3]
tags: [architecture, api-design, domain-modeling]
curated: 2026-06-16
curated_by: config-scout
---

# kase1111-hash/StreamTree — claude-md

**Why it's worth keeping:** It defines specific API response formats and a custom 'NFTree' domain model, which prevents an AI from hallucinating incorrect patterns or data structures during development.

**Summary:** A high-density architectural guide for a full-stack monorepo that bridges low-level file locations with high-level business domain logic.

**Source credibility:** Single star indicates a small/personal project, but the technical detail suggests it is not auto-generated.

**Recency:** Current; utilizes modern tech like Next.js 14 and ethers.js v6.

**Source:** [kase1111-hash/StreamTree/claude.md](https://github.com/kase1111-hash/StreamTree/blob/7d6d83c30d9bc7662e79bcc18ef50c2c8f510a44/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# StreamTree

StreamTree transforms passive streaming viewership into interactive, gamified participation with permanent collectible proof. Streamers create bingo-style games, and audience members mint cards that update live as events fire, culminating in permanent NFTs.

## Architecture

Turbo monorepo with npm workspaces:

- **apps/api**: Express.js backend with Prisma ORM, WebSocket for real-time updates
- **apps/web**: Next.js 14 frontend with React 18, Tailwind CSS, RainbowKit for Web3
- **packages/shared**: TypeScript types and utilities shared across apps
- **packages/contracts**: Solidity smart contracts (Hardhat)
- **packages/e2e-tests**: Integration tests (Vitest)

## Tech Stack

- **Backend**: Node.js, Express, Prisma, PostgreSQL 16, Redis 7, WebSocket
- **Frontend**: Next.js 14 (App Router), React 18, Tailwind CSS, Wagmi/Viem
- **Blockchain**: Solidity, Hardhat, ethers.js v6
- **Auth**: JWT (HTTP-only cookies), bcryptjs
- **Payments**: Stripe (with Connect for payouts)
- **Storage**: AWS S3

## Development

```bash
# Setup
docker-compose up -d              # Start PostgreSQL + Redis
npm install
npm run db:generate && npm run db:push
npm run dev                       # A
```

</details>
