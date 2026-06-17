---
name: taikoxyz__taiko-mono
source: https://github.com/taikoxyz/taiko-mono/blob/027e6122b036b7a0590fe0b3503d57b0e80eecc4/CLAUDE.md
repo: taikoxyz/taiko-mono
kind: claude-md
stars: 4568
last_pushed: 2026-06-15T06:54:16Z
license: other
score: 9
domains: [blockchain, smart-contracts, monorepo, backend]
tags: [solidity, go, rust, pnpm, zk-evm]
curated: 2026-06-15
curated_by: config-scout
---

# taikoxyz/taiko-mono — claude-md

**Why it's worth keeping:** Features specific command patterns (pnpm filters), language-specific debugging toolchains, and highly structured documentation standards like the Solidity NatSpec requirements.

**Summary:** Provides a comprehensive blueprint for navigating and developing within a complex multi-language monorepo.

**Source credibility:** High; Taiko is a major Ethereum rollup protocol with significant social proof and active maintenance.

**Recency:** Current; utilizes modern monorepo workflows and contemporary development tooling.

**Source:** [taikoxyz/taiko-mono/CLAUDE.md](https://github.com/taikoxyz/taiko-mono/blob/027e6122b036b7a0590fe0b3503d57b0e80eecc4/CLAUDE.md) · 4568★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 🎯 Project Overview

Taiko is a based rollup on Ethereum that uses validity proofs for finalization. It's designed to be a type-1 (fully Ethereum-equivalent) ZK-EVM.

**Key Technical Aspects:**

- Based rollup architecture (L1-sequenced)
- Uses SGX and ZK proofs for block verification
- Multi-proof system supporting different proof tiers
- Contestable validity proofs with bonding mechanism
- Native Ethereum equivalence (type-1 ZK-EVM)

## 📦 Monorepo Architecture

```
packages/
├── protocol/           # Core smart contracts (Solidity, Foundry)
├── taiko-client/       # Go client (driver, proposer, prover)
├── taiko-client-rs/    # Rust client implementation
├── relayer/            # Bridge message relayer (Go)
├── eventindexer/       # Event indexing service (Go)
├── urcindexer-rs/      # URC indexer (Rust)
├── bridge-ui/          # Bridge frontend (SvelteKit)
└── [other packages]    # UIs, NFTs, monitoring, tools
```

**Technology Stack:**

- Smart contracts: Solidity + Foundry
- Backend services: Go, Rust
- Frontend applications: TypeScript/SvelteKit
- Package man
```

</details>
