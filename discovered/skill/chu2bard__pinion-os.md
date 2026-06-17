---
name: chu2bard__pinion-os
source: https://github.com/chu2bard/pinion-os/blob/24292698ad3766c9718acfd2cd467cf1472b4c6e/SKILL.md
repo: chu2bard/pinion-os
kind: skill
stars: 95
last_pushed: 2026-02-23T09:47:35Z
license: mit
score: 7
domains: [blockchain, ai-agents, web3]
tags: [base, crypto, micropayments]
curated: 2026-06-16
curated_by: config-scout
---

# chu2bard/pinion-os — skill

**Why it's worth keeping:** The architecture of providing individual SKILL.md files for each tool is an excellent pattern for managing complex, high-stakes API interactions with LLMs. It also demonstrates how to integrate economic agency (micropayments) into agent skill sets.

**Summary:** A granular skill framework for executing on-chain transactions and intelligence on the Base network using a paywalled micro-transaction model.

**Source credibility:** Moderate; 95 stars and recent activity suggest a functional niche protocol.

**Recency:** Current; leverages modern blockchain standards and evolving AI-agent patterns.

**Source:** [chu2bard/pinion-os/SKILL.md](https://github.com/chu2bard/pinion-os/blob/24292698ad3766c9718acfd2cd467cf1472b4c6e/SKILL.md) · 95★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pinion-chain-intel
description: On-chain intelligence, transactions and wallet tools on Base. 9 x402-paywalled skills at $0.01 USDC each.
---

# Pinion Chain Intel -- OpenClaw Skills

On-chain intelligence, transactions, wallet tools and an AI agent on Base, paywalled via x402 USDC micropayments.

**Server:** https://pinionos.com/skill/
**Price:** $0.01 USDC per call (x402 on Base)
**Free catalog:** `GET /skill/catalog`

## Skills

| # | Skill | Endpoint | Method | Description |
|---|-------|----------|--------|-------------|
| 1 | [balance](skills/balance/SKILL.md) | `/balance/:address` | GET | ETH and USDC balances for any Base address |
| 2 | [tx](skills/tx/SKILL.md) | `/tx/:hash` | GET | Decoded transaction details for any Base tx hash |
| 3 | [price](skills/price/SKILL.md) | `/price/:token` | GET | Current USD price for ETH, USDC, WETH, DAI, USDT, CBETH |
| 4 | [wallet](skills/wallet/SKILL.md) | `/wallet/generate` | GET | Generate a fresh Ethereum keypair for Base |
| 5 | [chat](skills/chat/SKILL.md) | `/chat` | POST | Chat with the Pinion AI agent (web search enabled) |
| 6 | [send](skills/send/SKILL.md) | `/send` | POST | Construct an unsigned ETH or USDC transfer
```

</details>
