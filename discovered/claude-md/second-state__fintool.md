---
name: second-state__fintool
source: https://github.com/second-state/fintool/blob/177a9b8e3a09e507cdb2c8458f2be4b9574abaaf/CLAUDE.md
repo: second-state/fintool
kind: claude-md
stars: 296
last_pushed: 2026-05-19T22:06:38Z
license: unknown
score: 9
domains: [cli-tools, fintech, rust, agents-ai]
tags: [rust, trading-cli, agentic-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# second-state/fintool — claude-md

**Why it's worth keeping:** Defines strict patterns for maintaining tool capabilities via a dedicated 'skills/' directory and mandates specific shell commands to prevent ambiguity during automated tasks.

**Summary:** Comprehensive guide that covers build/test protocols and architectural constraints while emphasizing agent-readability. It uniquely integrates a 'skills' documentation strategy for AI discovery.

**Source credibility:** High; well-structured Rust project with significant community traction (296 stars).

**Recency:** Current; specifically optimized for agentic workflows and modern developer tooling.

**Source:** [second-state/fintool/CLAUDE.md](https://github.com/second-state/fintool/blob/177a9b8e3a09e507cdb2c8458f2be4b9574abaaf/CLAUDE.md) · 296★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Fintool Development Guide

## Project Overview

Fintool is a suite of Rust CLI tools for agentic trading and market intelligence across multiple exchanges. Each exchange has its own dedicated binary. All CLIs support `--json` mode for scripting and AI agent integration.

**Supported exchanges**: Hyperliquid, Binance, Coinbase, OKX, Polymarket (prediction markets)
**Asset classes**: Crypto, stocks, commodities, indices, prediction markets
**License**: MIT

## Repository Structure

```
fintool/
├── src/
│   ├── lib.rs              # Library root — exports all modules
│   ├── bin/                 # Binary entry points (one per exchange + fintool + backtest)
│   │   ├── fintool.rs       # Market intelligence CLI (quotes, news, SEC filings)
│   │   ├── hyperliquid.rs   # Hyperliquid (spot, perp, HIP-3, deposits, withdrawals)
│   │   ├── binance.rs       # Binance (spot, perp, deposits, withdrawals)
│   │   ├── coinbase.rs      # Coinbase (spot, deposits, withdrawals)
│   │   ├── okx.rs           # OKX (spot, perp, deposits, withdrawals, transfers)
│   │   ├── polymarket.rs    # Polymarket (prediction market trading)
│   │   └── backtest.rs      # Historical simulation with
```

</details>
