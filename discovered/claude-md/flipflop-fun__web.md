---
name: flipflop-fun__web
source: https://github.com/flipflop-fun/web/blob/d7c952dec4f2bcb6c35970f02619a6fad3a432e6/CLAUDE.md
repo: flipflop-fun/web
kind: claude-md
stars: 2
last_pushed: 2026-03-22T14:07:42Z
license: unknown
score: 8
domains: [web-frontend, blockchain, solana]
tags: [pda-structures, solana, typescript, dapp]
curated: 2026-06-16
curated_by: config-scout
---

# flipflop-fun/web — claude-md

**Why it's worth keeping:** The inclusion of exact Program Derived Address (PDA) seeds provides essential domain intelligence that prevents LLM hallucinations; the strict communication and coding standards ensure high consistency.

**Summary:** Provides deep technical context for a Solana DApp, specifically detailing critical blockchain-specific PDA structures and development workflows.

**Source credibility:** Low star count, but demonstrates highly specialized, practical knowledge typical of production-grade DApp development.

**Recency:** Very recent (3 months ago), consistent with modern development practices.

**Source:** [flipflop-fun/web/CLAUDE.md](https://github.com/flipflop-fun/web/blob/d7c952dec4f2bcb6c35970f02619a6fad3a432e6/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## FlipFlop.plus Web Client

**Overview**: A cutting-edge decentralized application (DApp) built on the Solana blockchain for token management, liquidity operations, and social trading features.

**Tech Stack**: React 18.3.1 + TypeScript, Solana Web3.js, Anchor Framework, Tailwind CSS, Raydium SDK v2

## Development Commands

### Setup & Installation
```bash
# Install dependencies
yarn install

# Environment setup
cp .env.example .env
```

### Development Workflow
```bash
# Start development server
yarn start

# Build for production
yarn build

# Run tests
yarn test
```

### Environment Configuration
Set these in `.env`:
- `REACT_APP_ENV`: development/production
- `REACT_APP_NETWORK`: devnet/mainnet_beta
- `REACT_APP_DEVNET_RPC`: Custom devnet RPC
- `REACT_APP_MAINNET_RPC`: Custom mainnet RPC

## Code Architecture

### Core Systems
- **Blockchain Layer**: Solana Web3.js + Anchor Framework
- **Wallet Integration**: Solana Wallet Adapter (Phantom, Solflare, Mobile)
- **State Management**: Apollo Client for GraphQL, React hooks for local state
- **Storage**: Arweave/Iry
```

</details>
