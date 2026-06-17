---
name: graphprotocol__contracts
source: https://github.com/graphprotocol/contracts/blob/33933275dabdbf016c80acc68e654ebbe62dfe57/CLAUDE.md
repo: graphprotocol/contracts
kind: claude-md
stars: 372
last_pushed: 2026-06-12T11:28:29Z
license: gpl-2.0
score: 9
domains: [blockchain, smart-contracts, monorepo]
tags: [pnpm, solidity, hardhat, foundry]
curated: 2026-06-15
curated_by: config-scout
---

# graphprotocol/contracts — claude-md

**Why it's worth keeping:** It solves the 'monorepo navigation' problem by providing explicit commands for sub-packages; it also establishes mental models (Proxy/Governor patterns) that prevent Claude from suggesting non-standard code.

**Summary:** A highly detailed guide for a complex smart contract monorepo using pnpm, Hardhat, and Foundry. It provides specific paths for running tests across different packages and defines high-level architectural patterns.

**Source credibility:** High: The Graph is a major, well-maintained decentralized protocol with significant industry presence.

**Recency:** Very current: uses modern tools like Hardhat Ignition and Foundry.

**Source:** [graphprotocol/contracts/CLAUDE.md](https://github.com/graphprotocol/contracts/blob/33933275dabdbf016c80acc68e654ebbe62dfe57/CLAUDE.md) · 372★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is The Graph Protocol's smart contracts monorepo - a decentralized network for querying and indexing blockchain data. It uses pnpm workspaces to manage multiple packages.

## Key Commands

### Build and Development

```bash
# Install dependencies (uses pnpm)
pnpm install

# Build all packages
pnpm build

# Clean build artifacts
pnpm clean

# Deep clean (including node_modules)
pnpm clean:all
```

### Testing

```bash
# Run all tests
pnpm test

# Run tests with coverage
pnpm test:coverage

# Test a specific package
cd packages/<package-name> && pnpm test

# Test a single file (in contracts package)
cd packages/contracts && npx hardhat test test/<FILE_NAME>.ts

# Run Foundry tests (in horizon/subgraph-service)
cd packages/horizon && pnpm test

# Run integration tests
cd packages/horizon && pnpm test:integration

# Run deployment tests
cd packages/horizon && pnpm test:deployment
```

### Linting and Formatting

```bash
# Run all linters
pnpm lint

# Format code
pnpm format

# Individual linters
pnpm lint:ts        # TypeScript/JavaScript
pnp
```

</details>
