---
name: Uniswap__universal-router
source: https://github.com/Uniswap/universal-router/blob/020e1b786ad9a6bad924874752167934734ad1e1/CLAUDE.md
repo: Uniswap/universal-router
kind: claude-md
stars: 503
last_pushed: 2026-06-03T16:08:58Z
license: gpl-3.0
score: 7
domains: [smart-contracts, blockchain, web3]
tags: [self-updating, dependency-tracking, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# Uniswap/universal-router — claude-md

**Why it's worth keeping:** Includes a 'self-maintenance' pattern that instructs the AI agent on how to keep this file synchronized via specific commands when files change.

**Summary:** Provides structured project metadata including build scripts and dependency versions with a built-in maintenance protocol.

**Source credibility:** Extremely high; Uniswap is a premier DeFi institution.

**Recency:** Current; utilizes meta-instructions specifically designed for maintaining LLM context.

**Source:** [Uniswap/universal-router/CLAUDE.md](https://github.com/Uniswap/universal-router/blob/020e1b786ad9a6bad924874752167934734ad1e1/CLAUDE.md) · 503★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Universal Router

## Overview

Smart contracts for Uniswap's Universal Router - a flexible, modular routing contract that enables complex multi-hop swaps across Uniswap V2, V3, and V4 protocols. Built with Solidity using Hardhat and Foundry.

## Scripts

- `npm run compile` - Compile contracts with Hardhat and Forge
- `npm run test:hardhat` - Run Hardhat integration tests
- `npm run test:gas` - Run gas benchmarking tests with snapshots
- `npm run test:all` - Run all tests (Hardhat + Foundry)
- `npm run lint` - Format TypeScript and Solidity files
- `npm run lint:check` - Check formatting without changes
- `npm run prettier:fix` - Format TypeScript and JSON files

## Dependencies

<!-- AUTO-GENERATED - Updated by /update-claude-md -->

**Production:**
- **@openzeppelin/contracts** (5.0.2) - Secure smart contract library
- **@uniswap/v2-core** (1.0.1) - Uniswap V2 protocol core
- **@uniswap/v3-core** (1.0.0) - Uniswap V3 protocol core

**Development:**
- **hardhat** (2.22.14) - Ethereum development environment
- **@nomicfoundation/hardhat-foundry** (1.1.2) - Foundry integration for Hardhat
- **@uniswap/router-sdk** (^1.3.0) - SDK for routing logic
- **@uniswap/sdk-core** (^3.0.1) -
```

</details>
