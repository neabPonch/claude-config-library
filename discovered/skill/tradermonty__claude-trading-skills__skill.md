---
name: tradermonty__claude-trading-skills__skill
source: https://github.com/tradermonty/claude-trading-skills/blob/b5566100dfad877f81fbad172293e2195f451919/skills/pair-trade-screener/SKILL.md
repo: tradermonty/claude-trading-skills
kind: skill
stars: 1913
last_pushed: 2026-06-14T14:29:10Z
license: mit
score: 9
domains: [finance, quantitative-analysis, data-science]
tags: [statistical-arbitrage, trading, quant]
curated: 2026-06-15
curated_by: config-scout
---

# tradermonty/claude-trading-skills — skill

**Why it's worth keeping:** It provides specific mathematical implementation details—like ADF testing, beta/hedge ratio calculation, and half-life estimation—that transform a general LLM into a domain-expert quantitative researcher.

**Summary:** A high-fidelity procedural workflow for conducting statistical arbitrage through pair trading analysis.

**Source credibility:** High; the source repository is well-starred and actively maintained.

**Recency:** 

**Source:** [tradermonty/claude-trading-skills/skills/pair-trade-screener/SKILL.md](https://github.com/tradermonty/claude-trading-skills/blob/b5566100dfad877f81fbad172293e2195f451919/skills/pair-trade-screener/SKILL.md) · 1913★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pair-trade-screener
description: Statistical arbitrage tool for identifying and analyzing pair trading opportunities. Detects cointegrated stock pairs within sectors, analyzes spread behavior, calculates z-scores, and provides entry/exit recommendations for market-neutral strategies. Use when user requests pair trading opportunities, statistical arbitrage screening, mean-reversion strategies, or market-neutral portfolio construction. Supports correlation analysis, cointegration testing, and spread backtesting.
---

# Pair Trade Screener

## Overview

This skill identifies and analyzes statistical arbitrage opportunities through pair trading. Pair trading is a market-neutral strategy that profits from the relative price movements of two correlated securities, regardless of overall market direction. The skill uses rigorous statistical methods including correlation analysis and cointegration testing to find robust trading pairs.

**Core Methodology:**
- Identify pairs of stocks with high correlation and similar sector/industry exposure
- Test for cointegration (long-term statistical relationship)
- Calculate spread z-scores to identify mean-reversion opportunities
- Generate
```

</details>
