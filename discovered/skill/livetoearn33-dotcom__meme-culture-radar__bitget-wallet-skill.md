---
name: livetoearn33-dotcom__meme-culture-radar__bitget-wallet-skill
source: https://github.com/livetoearn33-dotcom/meme-culture-radar/blob/ae61ff57924b57f68de7c66ea68163a836352a77/BITGET-WALLET-SKILL.md
repo: livetoearn33-dotcom/meme-culture-radar
kind: skill
stars: 0
last_pushed: 2026-03-26T11:39:29Z
license: unknown
score: 9
domains: [finance, crypto-api, agent-workflows]
tags: [workflow-orchestration, protocol-driven, safety-checks]
curated: 2026-06-16
curated_by: config-scout
---

# livetoearn33-dotcom/meme-culture-radar — skill

**Why it's worth keeping:** It utilizes a 'Mandatory Domain Knowledge' pattern that forces the agent to load specific context files before execution, and it defines strict pre-flight check flows (balance/risk) to prevent errors in high-stakes transactions.

**Summary:** This skill provides a highly structured operational protocol for interacting with complex crypto-trading APIs through multi-step verification workflows.

**Source credibility:** Low public reputation (0 stars), but the sophisticated structure suggests professional-grade system prompting.

**Recency:** Highly relevant; demonstrates modern 'Chain of Thought' and tool-use orchestration patterns.

**Source:** [livetoearn33-dotcom/meme-culture-radar/BITGET-WALLET-SKILL.md](https://github.com/livetoearn33-dotcom/meme-culture-radar/blob/ae61ff57924b57f68de7c66ea68163a836352a77/BITGET-WALLET-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bitget-wallet
version: "2026.3.12-1"
updated: "2026-03-12"
description: "Interact with Bitget Wallet API for crypto market data, token info, swap quotes, RWA (real-world asset) stock trading, and security audits. Use when the user asks about wallet, token prices, market data, swap/trading quotes, RWA stock discovery and trading, token security checks, K-line charts, or token rankings on supported chains (ETH, SOL, BSC, Base, etc.)."
---

# Bitget Wallet Skill

## API Overview

**⚠️ MANDATORY: Load Domain Knowledge Before Any API Call**

**Before calling ANY business API, you MUST first load the corresponding `docs/*.md` file for that domain.** This is non-negotiable — domain knowledge contains critical flow rules, parameter constraints, and pitfalls that cannot be inferred from command syntax alone. Skipping this step leads to silent failures, incorrect parameters, or broken flows.

| Business Domain | Must Load First | Before Calling |
|----------------|----------------|----------------|
| Swap / Trade | [`docs/swap.md`](docs/swap.md) | quote, confirm, make-order, send, get-order-details |
| Market Data / Token Analysis | [`docs/market-data.md`](docs/market-data.md) | co
```

</details>
