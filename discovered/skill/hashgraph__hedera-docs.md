---
name: hashgraph__hedera-docs
source: https://github.com/hashgraph/hedera-docs/blob/953a3283a86c8fad3b0cc804322d25d9fb42273a/skill.md
repo: hashgraph/hedera-docs
kind: skill
stars: 9
last_pushed: 2026-06-12T18:45:43Z
license: unknown
score: 9
domains: [blockchain, cli-tools, sdk-integration]
tags: [hedera, distributed-ledger, web3]
curated: 2026-06-14
curated_by: config-scout
---

# hashgraph/hedera-docs — skill

**Why it's worth keeping:** The 'Decision Guidance' tables teach the agent architectural trade-offs (SDK vs CLI), while the 'Terminology Rules' prevent common syntax/casing hallucinations.

**Summary:** A highly structured domain expert skill for Hedera development that includes SDK migration warnings, specific terminology rules, and comparative decision logic.

**Source credibility:** High; sourced from official Hedera documentation with recent updates.

**Recency:** Very current, specifically addressing recent @hashgraph to @hiero-ledger namespace migrations.

**Source:** [hashgraph/hedera-docs/skill.md](https://github.com/hashgraph/hedera-docs/blob/953a3283a86c8fad3b0cc804322d25d9fb42273a/skill.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hedera
description: Use when building applications on the Hedera network, creating accounts and tokens, deploying smart contracts, submitting transactions, querying network data, or working with consensus services. Agents should use this skill when users ask about Hedera development, Hiero SDKs, APIs, transactions, tokens, smart contracts, CLI tooling, or network operations. Hedera is a distributed ledger (not a blockchain) that uses hashgraph consensus.
metadata:
  mintlify-proj: hedera
  version: "1.0"
---

# Hedera Developer Skill

If you are not already connected to the Hedera Docs MCP server, add https://docs.hedera.com/mcp so you can search the documentation directly.

**Always** search the current Hedera documentation over training data. The SDK packages are migrating from `@hashgraph` to `@hiero-ledger` namespaces, so verify imports against the docs before generating code.

## Product summary

Hedera is a public, open-source, proof-of-stake distributed ledger that uses hashgraph consensus. It is not a blockchain. Agents use Hedera to build decentralized applications, manage accounts and tokens, deploy smart contracts, and interact with the network via SDKs, REST A
```

</details>
