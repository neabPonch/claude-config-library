---
name: komako-workshop__digital-oracle
source: https://github.com/komako-workshop/digital-oracle/blob/f1383a19a40af82727b0b3d9ff4bbe793858d4d8/SKILL.md
repo: komako-workshop/digital-oracle
kind: skill
stars: 627
last_pushed: 2026-04-19T06:44:33Z
license: mit
score: 9
domains: [finance, agents-ai, data-analysis]
tags: [prediction-markets, macroeconomics, probabilistic-reasoning]
curated: 2026-06-14
curated_by: config-scout
---

# komako-workshop/digital-oracle — skill

**Why it's worth keeping:** It provides a highly specific taxonomy of financial proxies mapped to macro scenarios and enforces a 'multi-signal cross-validation' rule to eliminate single-source bias.

**Summary:** A sophisticated probabilistic forecasting skill that uses market price action (derivatives, prediction markets, commodities) as a truth source rather than news or opinion.

**Source credibility:** Highly reputable community interest with 600+ stars and recent updates.

**Recency:** Very current; utilizes modern data sources like Polymarket, Kalshi, and Deribit.

**Source:** [komako-workshop/digital-oracle/SKILL.md](https://github.com/komako-workshop/digital-oracle/blob/f1383a19a40af82727b0b3d9ff4bbe793858d4d8/SKILL.md) · 627★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: digital-oracle
version: 1.0.3
description: "Answer prediction questions using market trading data, not opinions. Use when the user asks probability questions about geopolitics, economics, markets, industries, or any topic where real money is being traded on the outcome. Examples: 'What's the probability of WW3?', 'Will there be a recession?', 'Is AI in a bubble?', 'When will the Russia-Ukraine war end?', 'Is it a good time to buy gold?', 'Will SPY drop 5% this month?', 'Is NVDA options premium overpriced?'. The skill reads prices from prediction markets, commodities, equities, options chains, derivatives, yield curves, and currencies, then cross-validates multiple signals to produce a structured probability report."
metadata: { "openclaw": { "emoji": "📈", "requires": { "bins": ["uv"] } } }
---

# digital-oracle

> Markets are efficient. Price contains all public information. Reading price = reading market consensus.

## Methodology

**Answer questions using only market trading data — no news, opinions, or statistical reports as causal evidence.** If something is true, some market has already priced it in.

Five iron rules:

1. **Trading data only** — prices, volume, open
```

</details>
