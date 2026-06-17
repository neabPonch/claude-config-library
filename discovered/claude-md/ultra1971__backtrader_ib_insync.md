---
name: ultra1971__backtrader_ib_insync
source: https://github.com/ultra1971/backtrader_ib_insync/blob/ff89f764706f60224e6ad9d38896daba1c8e2326/CLAUDE.md
repo: ultra1971/backtrader_ib_insync
kind: claude-md
stars: 79
last_pushed: 2026-02-28T01:19:55Z
license: gpl-3.0
score: 8
domains: [fintech, algorithmic-trading, python]
tags: [async, integration, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# ultra1971/backtrader_ib_insync — claude-md

**Why it's worth keeping:** The inclusion of 'Key Components' mapping class roles to logic, combined with a concrete usage pattern, allows an AI to write correct implementations without guesswork. The technical warnings about singletons and async event loop constraints prevent common integration errors.

**Summary:** This config provides a high-density architectural map of an async trading integration. It defines specific data contract formats and component responsibilities essential for accurate code generation.

**Source credibility:** Moderate; 79 stars indicates a legitimate, specialized tool used in the algo-trading community.

**Recency:** Current; updated within the last few months.

**Source:** [ultra1971/backtrader_ib_insync/CLAUDE.md](https://github.com/ultra1971/backtrader_ib_insync/blob/ff89f764706f60224e6ad9d38896daba1c8e2326/CLAUDE.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

`backtrader_ib_insync` is a Python library that integrates Interactive Brokers (IB) with the [Backtrader](https://www.backtrader.com/) algorithmic trading framework, using the modern `ib_insync` async API. It provides a live trading data feed, broker interface, and data store for connecting Backtrader strategies directly to IB TWS or IB Gateway.

## Project Structure

```
backtrader_ib_insync/
├── backtrader_ib_insync/
│   ├── __init__.py      # Package exports: IBStore, IBBroker, IBData
│   ├── ibstore.py       # IBStore — singleton IB connection & data/order coordination
│   ├── ibbroker.py      # IBBroker — Backtrader broker interface + IBOrder/IBCommInfo
│   └── ibdata.py        # IBData — data feed (real-time bars, RTVolume, historical)
├── examples/
│   └── ibdemo.py        # Demo strategy using EUR.USD historical data
├── requirements.txt     # ib_insync
└── setup.py             # Package metadata (version 0.0.1, Python >=3.6)
```

## Key Components

### IBStore (`ibstore.py`)
- **Singleton** — one IB connection per process
- Wraps `ib_insync.IB`; manages connection, reconnection, and time sync
- Handles historical data requests (with smart
```

</details>
