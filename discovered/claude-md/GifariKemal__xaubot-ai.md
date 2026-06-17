---
name: GifariKemal__xaubot-ai
source: https://github.com/GifariKemal/xaubot-ai/blob/10301c8665443d2b83569840df65de49b6890cbe/CLAUDE.md
repo: GifariKemal/xaubot-ai
kind: claude-md
stars: 40
last_pushed: 2026-02-11T16:37:19Z
license: mit
score: 9
domains: [trading-bots, machine-learning, fintech]
tags: [algorithmic-trading, mlops, async-python]
curated: 2026-06-15
curated_by: config-scout
---

# GifariKemal/xaubot-ai — claude-md

**Why it's worth keeping:** The 'Architecture' workflow provides a step-by-step mental model for the AI, while the technical constraints preemptively correct likely library misuse (e.g., Polars vs Pandas).

**Summary:** Detailed documentation of an async ML trading loop, mapping specific data flows from market capture to trade execution.

**Source credibility:** High; reflects a sophisticated, multi-component system with clear architectural logic.

**Recency:** Current; utilizes modern Python 3.11+ and recent data engineering patterns.

**Source:** [GifariKemal/xaubot-ai/CLAUDE.md](https://github.com/GifariKemal/xaubot-ai/blob/10301c8665443d2b83569840df65de49b6890cbe/CLAUDE.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — XAUBot AI

## Project Overview

XAUBot AI is an automated XAUUSD (Gold) trading bot that combines Machine Learning (XGBoost), Smart Money Concepts (SMC), and Hidden Markov Model (HMM) regime detection. It runs on MetaTrader 5 via an async Python loop, executing trades on M15 candles.

## Directory Structure

```
.
├── main_live.py              # Main async trading orchestrator
├── train_models.py           # Model training script
├── Dockerfile                # Docker image (must be at root)
├── docker-compose.yml        # Docker orchestration (must be at root)
├── .dockerignore             # Docker build exclusions (must be at root)
├── src/                      # Core modules
│   ├── config.py             # Trading configuration & capital modes
│   ├── mt5_connector.py      # MetaTrader 5 connection layer
│   ├── smc_polars.py         # Smart Money Concepts (Polars-based)
│   ├── ml_model.py           # XGBoost trading model
│   ├── feature_eng.py        # Feature engineering (37 features)
│   ├── regime_detector.py    # HMM market regime detection
│   ├── risk_engine.py        # Risk calculations & validation
│   ├── smart_risk_manager.py # Dynamic risk management
```

</details>
