---
name: kase1111-hash__Pledge-Protocol
source: https://github.com/kase1111-hash/Pledge-Protocol/blob/21a7aba97a1cc9e7f55230e48a7f644f0cc67d81/claude.md
repo: kase1111-hash/Pledge-Protocol
kind: claude-md
stars: 1
last_pushed: 2026-02-23T16:43:13Z
license: mit
score: 9
domains: [blockchain, smart-contracts, backend-api]
tags: [solidity, typescript, architecture, escrow]
curated: 2026-06-16
curated_by: config-scout
---

# kase1111-hash/Pledge-Protocol — claude-md

**Why it's worth keeping:** It uses code snippets to demonstrate mandatory design patterns (e.g., Zod validation/Oracle providers) rather than just describing them, ensuring AI adherence.

**Summary:** A high-density technical blueprint that defines specific architectural patterns and implementation standards for a blockchain project.

**Source credibility:** Low star count, but demonstrates high technical documentation rigor.

**Recency:** Highly current with up-to-date tool versions and modern TypeScript practices.

**Source:** [kase1111-hash/Pledge-Protocol/claude.md](https://github.com/kase1111-hash/Pledge-Protocol/blob/21a7aba97a1cc9e7f55230e48a7f644f0cc67d81/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - Pledge Protocol

## Project Overview

Pledge Protocol is a milestone-verified crowdfunding platform built on blockchain. Money is locked in escrow until external oracles verify milestone completion (race results, academic records, GitHub commits, etc.). Backers receive Pledge Tokens during campaigns and soulbound Commemorative Tokens after resolution.

**Version**: 0.1.0
**License**: MIT
**Node**: 20.x LTS

## Tech Stack

### Smart Contracts
- Solidity 0.8.24 with OpenZeppelin v5.0.0
- Hardhat 2.19.0 for development/testing/deployment
- Ethers.js v6.9.0 with TypeChain bindings

### Backend
- TypeScript 5.3 (strict mode)
- Express.js 4.18
- Zod 3.22 for validation
- PostgreSQL database

### Testing
- Mocha/Chai via Hardhat
- 13 test suites covering all phases

## Directory Structure

```
contracts/           # Solidity smart contracts
  ├── CampaignRegistry.sol    # Campaign lifecycle
  ├── PledgeManager.sol       # Pledge management
  ├── EscrowVault.sol         # Fund escrow
  ├── OracleRegistry.sol      # Oracle management
  └── tokens/                 # ERC-721/ERC-5192 tokens

src/
  ├── api/routes/    # Express API endpoints (18 routes)
  ├── oracle/        # Ora
```

</details>
