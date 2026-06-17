---
name: solana-foundation__solana-dev-skill__skill
source: https://github.com/solana-foundation/solana-dev-skill/blob/99be3ef2b55587cbf4cab2bd346160eb75e944a0/skill/SKILL.md
repo: solana-foundation/solana-dev-skill
kind: skill
stars: 521
last_pushed: 2026-06-12T17:55:23Z
license: mit
score: 10
domains: [blockchain, smart-contracts, security, cli-tools]
tags: [solana, web3, rust, security]
curated: 2026-06-15
curated_by: config-scout
---

# solana-foundation/solana-dev-skill — skill

**Why it's worth keeping:** Uses opinionated tech-stack defaults to prevent agent drift and includes advanced safety guardrails like the NO_DNA CLI standard and data validation patterns.

**Summary:** A comprehensive development playbook that mandates specific high-performance libraries and provides strict security protocols for Solana programming.

**Source credibility:** Extremely high; official documentation/skill provided by the Solana Foundation.

**Recency:** Very current, reflecting modern @solana/kit standards rather than legacy web3.js patterns.

**Source:** [solana-foundation/solana-dev-skill/skill/SKILL.md](https://github.com/solana-foundation/solana-dev-skill/blob/99be3ef2b55587cbf4cab2bd346160eb75e944a0/skill/SKILL.md) · 521★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: solana-dev
description: Use when user asks to "build a Solana dapp", "write an Anchor program", "create a token", "debug Solana errors", "set up wallet connection", "test my Solana program", "deploy to devnet", or "explain Solana concepts" (rent, accounts, PDAs, CPIs, etc.). Also use for quick on-chain lookups via public RPC + curl — "what's the balance of <wallet>", "look up transaction <sig>", "token balance for <account>", "check this address on mainnet/devnet". End-to-end Solana development playbook covering wallet connection, Anchor/Pinocchio programs, Codama client generation, LiteSVM/Mollusk/Surfpool testing, security checklists, and JSON-RPC curl lookups against public clusters. Integrates with the Solana MCP server for live documentation search. Prefers framework-kit (@solana/client + @solana/react-hooks) for UI, wallet-standard-first connection (incl. ConnectorKit), @solana/kit for client/RPC code, and @solana/web3-compat for legacy boundaries.
user-invocable: true
license: MIT
compatibility: Requires Node.js 18+, Rust toolchain, Solana CLI, Anchor CLI
metadata:
  author: Solana Foundation
  version: 1.2.0
---

# Solana Development Skill (framework-kit-first)

#
```

</details>
