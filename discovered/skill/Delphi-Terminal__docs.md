---
name: Delphi-Terminal__docs
source: https://github.com/Delphi-Terminal/docs/blob/6a8d78b350b2dfffff156fdef37b004a7733fc32/skill.md
repo: Delphi-Terminal/docs
kind: skill
stars: 0
last_pushed: 2026-05-01T14:35:31Z
license: mit
score: 9
domains: [api-integration, trading, agents-ai]
tags: [prediction-markets, rest-api, technical-documentation]
curated: 2026-06-14
curated_by: config-scout
---

# Delphi-Terminal/docs — skill

**Why it's worth keeping:** The 'Bootstrap flow' (enabling self-starting via curl) and the detailed identifier mapping table are elite techniques that prevent agent errors during path construction. It serves as an excellent template for turning complex documentation into actionable tool instructions.

**Summary:** A high-density API skill definition for interacting with a multi-exchange prediction market aggregator. It provides structured paths, authentication logic, and exchange-specific identifiers.

**Source credibility:** Low social proof/stars, but high technical density suggests it is a professional developer-led document.

**Recency:** Highly current; follows modern best practices for LLM tool-use and agentic workflows.

**Source:** [Delphi-Terminal/docs/skill.md](https://github.com/Delphi-Terminal/docs/blob/6a8d78b350b2dfffff156fdef37b004a7733fc32/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: delphi-terminal
description: Query unified prediction market data (Kalshi, Polymarket, Limitless, Predict.fun, Gemini, Manifold, Opinion, ForecastEx, PredictIt) and parlay RFQs/trades via the Delphi Terminal API.
triggers:
  - prediction market
  - Kalshi / KLSI
  - Polymarket / POLY
  - Limitless, Predict.fun, Gemini, Manifold, Opinion, ForecastEx, PredictIt
  - market odds, prices, orderbook, trade history, OHLCV candles
  - RFQ, MVE trades, parlays
---

# Delphi Terminal API — Agent Skill

You are about to query the Delphi Terminal API, a single interface for prediction market data across nine exchanges and a parlays/RFQ feed. This file is the authoritative guide. Follow it literally.

## When to use this skill

Use this skill whenever the user asks about:

- Prediction market odds, prices, volume, liquidity, spreads
- Orderbooks, top-of-book, raw orderbook deltas
- Trade history or OHLCV candles
- Market search, semantic search, categories, events, clusters
- Parlay RFQs, MVE trades
- Bulk historical data exports (parquet)
- Real-time streaming via WebSockets

If the user names any of these exchanges or asks for "live odds," default to this skill:
**Kalshi, Polymarket
```

</details>
