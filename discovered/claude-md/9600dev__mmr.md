---
name: 9600dev__mmr
source: https://github.com/9600dev/mmr/blob/07559fb9eebcdc88c466569b9b36a112842af547/CLAUDE.md
repo: 9600dev/mmr
kind: claude-md
stars: 121
last_pushed: 2026-05-17T03:48:10Z
license: other
score: 9
domains: [algorithmic-trading, backend-systems, distributed-systems]
tags: [zmq, duckdb, architecture-patterns, high-precision]
curated: 2026-06-15
curated_by: config-scout
---

# 9600dev/mmr — claude-md

**Why it's worth keeping:** The breakdown of three distinct messaging patterns (RPC, PubSub, MessageBus) and the detailed dependency injection implementation provide an elite mental model for LLMs to navigate complex system interactions.

**Summary:** Defines an algorithmic trading architecture centered on ZMQ-based inter-process communication and DuckDB storage. It prioritizes extreme precision, explicit error handling, and specific data sourcing rules.

**Source credibility:** Highly credible; demonstrated by a specialized trading platform with significant GitHub stars.

**Recency:** Current; utilizes modern Python patterns including asyncio, ZMQ, and DuckDB.

**Source:** [9600dev/mmr/CLAUDE.md](https://github.com/9600dev/mmr/blob/07559fb9eebcdc88c466569b9b36a112842af547/CLAUDE.md) · 121★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

MMR (Make Me Rich) is a Python-based algorithmic trading platform for Interactive Brokers. It supports automated strategy execution, interactive CLI trading, historical data collection, real-time market data streaming, and idea scanning across US and international markets.

## Design Principles

**Precision over convenience**: This is a trading system — wrong data is worse than no data. Contract identifiers (conIds) must resolve exactly or fail. Never fall back to fuzzy matching, string coercion, or "close enough" lookups. If a conId isn't found, return an error. If a symbol resolves to the wrong exchange, that's a bug. Integer conIds passed to `resolve_symbol` must not be converted to string symbol lookups (e.g. conId `4391` must not become ticker `"4391"` which matches a Japanese stock on TSEJ).

**Fail loudly, not silently**: When an IB API call fails (scanner error 162, market data not subscribed, contract not found), surface the error to the caller. Don't swallow exceptions and return empty results — the user needs to know *why* something failed so they can fix it (subscribe to market data, use a different location code, etc.).

**Massive firs
```

</details>
