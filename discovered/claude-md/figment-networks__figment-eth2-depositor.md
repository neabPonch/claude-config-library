---
name: figment-networks__figment-eth2-depositor
source: https://github.com/figment-networks/figment-eth2-depositor/blob/4b44370eca2bc3a0f80f6b5a95c63511adcc3c44/CLAUDE.md
repo: figment-networks/figment-eth2-depositor
kind: claude-md
stars: 3
last_pushed: 2026-04-21T17:21:57Z
license: mit
score: 9
domains: [smart-contracts, blockchain, ethereum]
tags: [solidity, hardhat, foundry, deployment-guide]
curated: 2026-06-15
curated_by: config-scout
---

# figment-networks/figment-eth2-depositor — claude-md

**Why it's worth keeping:** Includes exact, long-form shell commands and critical business logic constants to prevent AI hallucinations during high-stakes tasks like contract verification or limit validation.

**Summary:** Provides precise, complex CLI commands for deployment and verification alongside a dual-framework architecture overview.

**Source credibility:** High; comes from Figment Networks, a major Ethereum infrastructure provider.

**Recency:** Highly current, referencing Hardhat 3 and the latest EVM 'Cancun' specifications.

**Source:** [figment-networks/figment-eth2-depositor/CLAUDE.md](https://github.com/figment-networks/figment-eth2-depositor/blob/4b44370eca2bc3a0f80f6b5a95c63511adcc3c44/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Solidity smart contract for batch Ethereum 2.0 validator deposits supporting variable amounts (1–2048 ETH per validator, up to 500 validators per transaction). Built with Hardhat 3 + Foundry dual-framework setup.

## Commands

```bash
# Install dependencies
pnpm install

# Run all tests (Forge + Node.js)
pnpm hardhat test

# Run only Solidity (Forge) tests
pnpm hardhat test solidity

# Run only Node.js tests
pnpm hardhat test nodejs

# Run a specific test file
pnpm hardhat test test/FigmentEth2DepositorV1.ts

# Deploy locally
pnpm hardhat ignition deploy ignition/modules/FigmentEth2DepositorV1.ts

# Deploy to Hoodi testnet (requires HOODI_PRIVATE_KEY in keystore)
pnpm hardhat keystore set HOODI_PRIVATE_KEY
pnpm hardhat ignition deploy --network hoodi ignition/modules/FigmentEth2DepositorV1.ts

# Contract verification (Hoodi)
forge build --force
forge verify-contract <address> contracts/FigmentEth2DepositorV1.sol:FigmentEth2DepositorV1 \
  --chain-id 560048 --etherscan-api-key <api-key> --constructor-args <encoded-args> \
  --optimizer-runs 200 --
```

</details>
