---
name: Adityaadpandey__Veris
source: https://github.com/Adityaadpandey/Veris/blob/91531ffd6d4d52291a5c8efa58b6a9f669d4f11f/claude.md
repo: Adityaadpandey/Veris
kind: claude-md
stars: 2
last_pushed: 2026-06-15T17:16:58Z
license: unknown
score: 9
domains: [web3, hardware, fullstack, blockchain]
tags: [monorepo-style, architectural-flow, hardware-integration]
curated: 2026-06-15
curated_by: config-scout
---

# Adityaadpandey/Veris — claude-md

**Why it's worth keeping:** The text-based data flow diagram and service-specific command groupings prevent context confusion in multi-directory repos. It also explicitly lists technology rationales (e.g., why ERC-1155 was used) which helps the AI make informed decisions.

**Summary:** Provides an exhaustive technical map of a complex hardware-integrated Web3 system, connecting local camera capture to blockchain events.

**Source credibility:** Low star count, but the level of technical specificity suggests a real-world engineering project.

**Recency:** Highly current; uses modern toolchains like Wagmi 2, Viem 2, and Foundry.

**Source:** [Adityaadpandey/Veris/claude.md](https://github.com/Adityaadpandey/Veris/blob/91531ffd6d4d52291a5c8efa58b6a9f669d4f11f/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Veris is a Web3 camera system that creates verifiable, blockchain-backed photo NFTs using Raspberry Pi hardware, Zero-Knowledge proofs, and Filecoin storage. The core value proposition: hardware-signed images + ZK proofs = verifiable proof a photo isn't AI-generated.

## Repository Structure

| Directory | Purpose |
|-----------|---------|
| `hardware-camera-app/` | Python/Kivy GUI on Raspberry Pi for camera capture |
| `hardware-web3-service/` | Node.js backend for Filecoin upload, ZK proofs, NFT minting |
| `lensmint-public-server/` | Node.js claim server with SQLite, generates QR codes |
| `owner-portal/` | React/Vite dashboard for users to claim/mint NFTs |
| `contracts/` | Solidity smart contracts with Foundry toolchain |

## Commands

### Owner Portal (React)
```bash
cd owner-portal
npm install
npm run dev       # Dev server on port 3000
npm run build     # Production build
npm run preview   # Preview production build
```

### Hardware Web3 Service (Node.js)
```bash
cd hardware-web3-service
npm install
npm run dev       # nodemon dev server
```

</details>
