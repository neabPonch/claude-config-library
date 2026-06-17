---
name: bnb-chain__bep-677-contracts
source: https://github.com/bnb-chain/bep-677-contracts/blob/ff17399a4723e2e344f7d4c52a3eecf2ca007f6b/CLAUDE.md
repo: bnb-chain/bep-677-contracts
kind: claude-md
stars: 0
last_pushed: 2026-05-08T02:35:52Z
license: mit
score: 8
domains: [blockchain, smart-contracts]
tags: [solidity, hardhat, deployment-safety]
curated: 2026-06-17
curated_by: config-scout
---

# bnb-chain/bep-677-contracts — claude-md

**Why it's worth keeping:** The explicit 'Do NOT deploy' convention is vital for agentic workflows, and the distinction between upgradeable vs. non-upgradeable paths prevents logic errors.

**Summary:** Provides structured technical context, command references, and critical deployment safety protocols for a Solidity/Hardhat project.

**Source credibility:** High; part of an official BNB Chain ecosystem repository.

**Recency:** Current; utilizes modern Hardhat and Solidity patterns.

**Source:** [bnb-chain/bep-677-contracts/CLAUDE.md](https://github.com/bnb-chain/bep-677-contracts/blob/ff17399a4723e2e344f7d4c52a3eecf2ca007f6b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# BEP-677 Contracts

Solidity smart contract project implementing BEP-677 (EIP-8056 Scaled UI Amount) on BNB Chain.

## Tech Stack

- **Hardhat** — Solidity 0.8.24, optimizer enabled (200 runs)
- **npm** — root project package manager
- **Bun** — playground/ subproject package manager

## Key Commands

```bash
npx hardhat compile      # compile contracts
npx hardhat test         # run tests
npx hardhat node         # start local node
```

## Project Structure

- `contracts/` — Solidity sources
  - `ERC8056Base.sol` — non-upgradeable abstract base (deprecated, reference only)
  - `ERC8056Token.sol` — concrete non-upgradeable token (`ScaledUIToken`, deprecated)
  - `ERC8056BaseUpgradeable.sol` — abstract Beacon-upgradeable base (inherit to extend)
  - `ERC8056TokenUpgradeable.sol` — concrete Beacon-upgradeable token (recommended, deploy directly)
  - `contracts/mocks/` — test mock contracts (not for production)
  - interfaces: `IScaledUIAmount*.sol`, `IERC8056Scheduled.sol`
- `abis/` — pre-built ABI JSON files
- `scripts/` — deploy scripts (`deploy.js`, `deploy-upgradeable.js`)
- `test/` — Hardhat test suite
- `playground/` — Vite + React frontend demo (separate Bun project)

## Depl
```

</details>
