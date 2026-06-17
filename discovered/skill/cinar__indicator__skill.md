---
name: cinar__indicator__skill
source: https://github.com/cinar/indicator/blob/7cba43f3e3f507d610758821b2ba35bd38114771/.gemini/skills/add-indicator/SKILL.md
repo: cinar/indicator
kind: skill
stars: 1155
last_pushed: 2026-06-08T12:58:44Z
license: agpl-3.0
score: 9
domains: [fintech, backend-go, data-streaming]
tags: [go, technical-analysis, concurrency, indicators]
curated: 2026-06-15
curated_by: config-scout
---

# cinar/indicator — skill

**Why it's worth keeping:** Defines a mandatory interface signature (Compute/IdlePeriod) and specific testing protocols to prevent common concurrency deadlocks in streaming data.

**Summary:** Provides strict architectural constraints for implementing new technical indicators using Go generics and channel-based streaming patterns.

**Source credibility:** High; high star count and very recent maintenance activity indicate a production-ready codebase.

**Recency:** Current; utilizes modern Go patterns like generics and sophisticated channel orchestration.

**Source:** [cinar/indicator/.gemini/skills/add-indicator/SKILL.md](https://github.com/cinar/indicator/blob/7cba43f3e3f507d610758821b2ba35bd38114771/.gemini/skills/add-indicator/SKILL.md) · 1155★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: add-indicator
description: Add a new technical analysis indicator to the project. Use when you need to implement a new indicator (e.g., SMA, EMA, RSI) following the project's streaming data patterns, Go generics, and channel-based API.
---

# Add Indicator

This skill provides the workflow and standards for adding new technical analysis indicators to the `indicator` project.

## Workflow

### 1. Identify Category and Location
Indicators are organized by their technical analysis category. Determine where the new indicator belongs:
- `trend/`: Trend-following indicators (SMA, EMA, MACD, etc.)
- `momentum/`: Momentum indicators (RSI, Stochastic, etc.)
- `volatility/`: Volatility indicators (Bollinger Bands, ATR, etc.)
- `volume/`: Volume-based indicators (OBV, Chaikin Money Flow, etc.)
- `valuation/`: Asset valuation (FV, NPV, etc.)

### 2. Implementation Standards

#### Streaming Data Patterns
- Indicators MUST operate on unlimited data streams using Go routines and channels.
- Use `<-chan T` for inputs and `<-chan T` (or multiple channels) for outputs.
- Indicators may have an "idle" or "warm-up" period where they don't produce output until their internal window is filled.
```

</details>
