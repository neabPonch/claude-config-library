---
name: tony1908__taller-monad
source: https://github.com/tony1908/taller-monad/blob/4905888d2957b5d5bb5fc565e333c972f0722c5d/CLAUDE.md
repo: tony1908/taller-monad
kind: claude-md
stars: 0
last_pushed: 2025-08-23T00:58:45Z
license: unknown
score: 9
domains: [mobile-app, web3, blockchain]
tags: [react-native, ethers.js, web3modal, smart-contracts]
curated: 2026-06-15
curated_by: config-scout
---

# tony1908/taller-monad — claude-md

**Why it's worth keeping:** The 'Smart Contract Integration Pattern' section provides explicit, high-value code comparisons to prevent common library-specific errors that LLMs often make.

**Summary:** A highly detailed project guide for a React Native Web3 application, covering environment setup, component architecture, and blockchain integration.

**Source credibility:** While the repository has low social proof (0 stars), the technical specificity suggests a well-engineered demo project.

**Recency:** 10 months old; remains highly relevant for modern React Native and Ethers.js development.

**Source:** [tony1908/taller-monad/CLAUDE.md](https://github.com/tony1908/taller-monad/blob/4905888d2957b5d5bb5fc565e333c972f0722c5d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a React Native Web3 application that demonstrates a staking-based Todo List system on Monad testnet. Users must stake native MON tokens to create todo items and get their stake back when they complete tasks. The app showcases Web3Modal (AppKit) integration with Ethers.js for blockchain wallet connections and smart contract interactions.

## Key Architecture

- **Web3 Integration**: Uses Reown's AppKit (formerly Web3Modal) with Ethers.js provider
- **Wallet Support**: Supports multiple wallet connections including WalletConnect, Coinbase, and custom wallets
- **Chain Configuration**: Currently configured for Monad testnet (chainId: 10143) with mainnet and Polygon available as alternatives
- **Authentication**: Includes SIWE (Sign-In with Ethereum) support via AuthProvider
- **Storage**: Uses MMKV for secure local storage

## Development Commands

### Dependency Installation
```bash
# Recommended: Use yarn (handles React Native dependencies better)
yarn install

# Alternative: Use npm with legacy peer deps
npm install --legacy-peer-deps

#
```

</details>
