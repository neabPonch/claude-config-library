---
name: agnij-dutta__FLIP
source: https://github.com/agnij-dutta/FLIP/blob/8856ff2b6b4de1d27fc45971b35711cdc49a24a1/claude.md
repo: agnij-dutta/FLIP
kind: claude-md
stars: 1
last_pushed: 2026-01-31T11:05:00Z
license: mit
score: 9
domains: [blockchain, smart-contracts, backend-agents, web-frontend]
tags: [monorepo, crypto, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# agnij-dutta/FLIP — claude-md

**Why it's worth keeping:** Includes high-value 'Key Design Decisions' that prevent AI from proposing logic changes that violate the intended economic model. The ASCII architecture diagram and specific build/test commands provide perfect context for an autonomous agent.

**Summary:** A comprehensive technical overview of a cross-chain settlement protocol spanning Solidity smart contracts, Go agents, and Next.js frontend.

**Source credibility:** Low star count but professionally authored technical documentation typical of serious blockchain infrastructure projects.

**Recency:** Very current, utilizing modern tech stacks like Next.js 14 and Wagmi 2.0.

**Source:** [agnij-dutta/FLIP/claude.md](https://github.com/agnij-dutta/FLIP/blob/8856ff2b6b4de1d27fc45971b35711cdc49a24a1/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FLIP - Flare Liquidity-Optimized Interoperability Protocol

## Overview

FLIP is a **conditional settlement acceleration layer** for Flare's FAssets. It solves the speed problem (FAsset redemptions take 3-5 minutes due to FDC latency) by providing near-instant user experience while preserving Flare's trust-minimized security model.

**Key Innovation**: FLIP v2 uses an escrow-based conditional settlement model instead of prefunded insurance pools, achieving 10-20x capital efficiency.

**NOT a bridge** - it's a settlement acceleration layer using State Connector (FDC) as the final arbiter.

## Architecture

```
┌─────────────────────────────────────────────────────┐
│         ON-CHAIN LAYER (Solidity 0.8.24)            │
│  FLIPCore → EscrowVault → SettlementReceipt (NFT)   │
│  LiquidityProviderRegistry | DeterministicScoring   │
│  OperatorRegistry | PriceHedgePool | OracleRelay    │
└─────────────────────────────────────────────────────┘
         ↕ (Events & RPC)
┌─────────────────────────────────────────────────────┐
│         AGENT LAYER (Go)                            │
│  EventMonitor → PaymentProcessor → FDCSubmitter     │
└──────────────────────────────────────────────────
```

</details>
