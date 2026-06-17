---
name: ricequant__rqalpha
source: https://github.com/ricequant/rqalpha/blob/745d81cf11c7f620f1aec7f7b1447b26796f79be/CLAUDE.md
repo: ricequant/rqalpha
kind: claude-md
stars: 6478
last_pushed: 2026-06-12T02:31:52Z
license: other
score: 9
domains: [fintech, python, trading-systems]
tags: [algorithmic-trading, backtesting, event-driven]
curated: 2026-06-15
curated_by: config-scout
---

# ricequant/rqalpha — claude-md

**Why it's worth keeping:** Includes critical constraints like stock code/date formats and maps specific documentation paths to different developer tasks (architecture vs. strategy writing). It also provides actionable debugging heuristics such as using short date ranges for faster iteration.

**Summary:** Provides highly specific domain knowledge for an algorithmic trading framework, including data formats, strategy lifecycles, and architectural patterns.

**Source credibility:** High-quality repository with significant stars and extremely recent maintenance activity.

**Recency:** Highly current; the structure is optimized for modern LLM-based coding agents.

**Source:** [ricequant/rqalpha/CLAUDE.md](https://github.com/ricequant/rqalpha/blob/745d81cf11c7f620f1aec7f7b1447b26796f79be/CLAUDE.md) · 6478★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

RQAlpha is an algorithmic trading system for quantitative trading with backtesting and live trading capabilities.

**License**: Non-commercial use only (Apache 2.0). Commercial use requires authorization from Ricequant.

## Quick Commands

```bash
# Run backtest
rqalpha run -f strategy.py -s 2014-01-01 -e 2016-01-01 --account stock 100000

# With RQData connection
rqalpha run --rqdatac-uri tcp://user:password@host:port -f strategy.py -s 2014-01-01 -e 2016-01-01 --account stock 100000

# Download bundle data
rqalpha download-bundle

# Update bundle
rqalpha update-bundle --rqdatac-uri tcp://user:password@host:port

# Generate examples
rqalpha examples -d ./examples

# Run tests
pytest
pytest tests/unittest/
pytest tests/integration_tests/
```

## Project-Specific Rules

### When Writing Strategies

1. **Always consult documentation first**: Read `docs/source/intro/tutorial.rst` and `docs/source/api/base_api.rst` before writing strategies
2. **Use correct API signatures**: Check `docs/source/api/base_api.rst` for function parameters and return types
3. **Follow strategy lifecycle**: Implement `init()`, `before_trading()`, `handle_bar()`, `after_trading()` in correct order
```

</details>
