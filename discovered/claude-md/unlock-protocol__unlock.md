---
name: unlock-protocol__unlock
source: https://github.com/unlock-protocol/unlock/blob/6e681fa5c4c793560e018382c8001cc00927f8b0/CLAUDE.md
repo: unlock-protocol/unlock
kind: claude-md
stars: 873
last_pushed: 2026-06-15T00:34:40Z
license: mit
score: 9
domains: [web3, blockchain, monorepo, smart-contracts, fullstack]
tags: [monorepo, solidity, nextjs, evm]
curated: 2026-06-15
curated_by: config-scout
---

# unlock-protocol/unlock — claude-md

**Why it's worth keeping:** It provides explicit context on workspace-specific command execution (cd into directory first) and high-level design patterns like 'Mixins' that prevent architectural hallucinations.

**Summary:** A comprehensive architectural and operational blueprint for a complex Web3 monorepo.

**Source credibility:** High; a mature, well-maintained protocol with significant community traction.

**Recency:** Extremely current; uses modern tech stacks and explicitly references Claude Code workflows.

**Source:** [unlock-protocol/unlock/CLAUDE.md](https://github.com/unlock-protocol/unlock/blob/6e681fa5c4c793560e018382c8001cc00927f8b0/CLAUDE.md) · 873★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Unlock Protocol Monorepo

Unlock is a decentralized membership/subscription protocol on EVM blockchains. NFT-based access control: **Locks** are smart contracts, **Keys** are NFTs granting membership.

## Monorepo Structure

Yarn 4.10.3 workspaces, Node >= 20 required, TypeScript throughout.

**Applications:**
- `unlock-app/` — Main dashboard (Next.js 14, Privy auth, ethers.js v6, React Query, Tailwind)
- `locksmith/` — Backend API (Express 5, Sequelize/Postgres, Graphile Worker jobs)
- `governance-app/` — DAO governance UI
- `wedlocks/` — Email service (Cloudflare Worker, Handlebars)
- `paywall-app/` — Embeddable paywall widget (Next.js, static export)
- `provider/` — RPC proxy (Cloudflare Worker, multi-chain rate limiting)
- `unlock-protocol-com/` — Marketing site (Docusaurus)

**Core:**
- `smart-contracts/` — Solidity (Hardhat, OpenZeppelin upgradeable proxies)
- `subgraph/` — The Graph indexer (AssemblyScript, GraphQL)
- `governance/` — DAO tooling (proposals, voting, cross-chain)
- `packages/` — 14 shared npm packages (networks, ui, unlock-js, contracts, etc.)

## Essential Commands

```bash
yarn                                             # Install all deps
yarn build
```

</details>
