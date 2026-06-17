---
name: MikeMoulder__eBidz
source: https://github.com/MikeMoulder/eBidz/blob/bb1a32965ec3d6631a758d33114e421d2b6a4a6a/skill.md
repo: MikeMoulder/eBidz
kind: skill
stars: 0
last_pushed: 2026-05-14T13:00:12Z
license: unknown
score: 9
domains: [blockchain, security, solana]
tags: [mpc, arcium, anchor, encryption]
curated: 2026-06-16
curated_by: config-scout
---

# MikeMoulder/eBidz — skill

**Why it's worth keeping:** It provides specific error code resolutions (e.g., InvalidCUAmount), exact argument builder sequences, and a rigorous inspection checklist for cross-file consistency.

**Summary:** A highly specialized domain skill for integrating Arcium MPC circuits into Solana/Anchor applications.

**Source credibility:** Low GitHub visibility but exhibits high technical depth in niche Solana MPC development.

**Recency:** Highly current; pushed within the last month.

**Source:** [MikeMoulder/eBidz/skill.md](https://github.com/MikeMoulder/eBidz/blob/bb1a32965ec3d6631a758d33114e421d2b6a4a6a/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
```markdown
---
name: arcium-solana-mpc
description: Build, audit, and debug Arcium-powered Solana/Anchor apps with encrypted circuits, MXE setup, computation definitions, x25519 encryption, queue_computation callbacks, and frontend integration. Use for Arcium errors like InvalidArguments, ConstraintSeeds, AccountDidNotDeserialize, InvalidCUAmount, aborted MPC callbacks, stuck finalization, or encrypted bid/vote/settlement flows.
---

# Arcium Solana MPC Skill

Use this skill when working on Solana + Anchor projects that integrate Arcium MPC circuits.

## Core Rule

Prefer incremental encrypted state over giant batch circuits.

A strong Arcium app usually does this:

1. Initialize encrypted state with a small circuit.
2. Update that encrypted state per user action.
3. Finalize by revealing only the minimum public result.

Avoid passing huge arrays like `[Enc<Shared, Bid>; 64]` into one final circuit unless the circuit weight is proven safe.

## First Inspection Checklist

Check these files before changing logic:

- `Anchor.toml`
- `Arcium.toml`
- `programs/*/src/lib.rs`
- `encrypted-ixs/src/lib.rs`
- `build/*.weight`
- `build/*.arcis`
- `scripts/init-comp-def*`
- `scripts/check-clu
```

</details>
