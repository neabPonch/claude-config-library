---
name: minhoyoo-iotrust__WAIaaS__transactions-skill
source: https://github.com/minhoyoo-iotrust/WAIaaS/blob/7efab376f9f901c787ef92cb5a1cd7d3ff0d643c/skills/transactions.skill.md
repo: minhoyoo-iotrust/WAIaaS
kind: skill
stars: 26
last_pushed: 2026-04-25T03:11:55Z
license: mit
score: 9
domains: [blockchain, api-integration, agents-ai]
tags: [wallet, transactions, web3]
curated: 2026-06-17
curated_by: config-scout
---

# minhoyoo-iotrust/WAIaaS — skill

**Why it's worth keeping:** Provides excellent clarity on edge cases like amount conversion (human vs smallest unit), explicit policy prerequisites, and strict JSON schemas for various transaction types.

**Summary:** Comprehensive technical specification for executing multi-chain blockchain transactions via a specialized Wallet-as-a-Service API.

**Source credibility:** Niche repository with moderate stars and recent maintenance activity.

**Recency:** Highly relevant to current agent-to-API orchestration patterns.

**Source:** [minhoyoo-iotrust/WAIaaS/skills/transactions.skill.md](https://github.com/minhoyoo-iotrust/WAIaaS/blob/7efab376f9f901c787ef92cb5a1cd7d3ff0d643c/skills/transactions.skill.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "WAIaaS Transactions"
description: "All 6 transaction types (TRANSFER, TOKEN_TRANSFER, CONTRACT_CALL, APPROVE, BATCH, NFT_TRANSFER) with lifecycle management"
category: "api"
tags: [wallet, blockchain, solana, ethereum, ripple, xrp, xrpl, transactions, waiass]
version: "2.6.0-rc"
dispatch:
  kind: "tool"
  allowedCommands: ["curl"]
---

# WAIaaS Transactions

Complete reference for all 6 transaction types, lifecycle management, and policy interaction. All endpoints use base URL `http://localhost:3100`. Transaction endpoints require **sessionAuth** (`Authorization: Bearer <token>`) unless noted otherwise.

> AI agents must NEVER request the master password. Use only your session token.

## Permissions

### Agent (sessionAuth)
- Send all 6 transaction types via `POST /v1/transactions/send`
- Sign raw transactions via `POST /v1/transactions/sign`
- Query transaction status and history
- Renew session tokens

### Owner (ownerAuth -- SIWS/SIWE)
- Approve pending transactions via `POST /v1/transactions/{id}/approve`
- Reject pending transactions via `POST /v1/transactions/{id}/reject`

**Prerequisite:** Policy types (ALLOWED_TOKENS, CONTRACT_WHITELIST, APPROVED_SPENDERS) must b
```

</details>
