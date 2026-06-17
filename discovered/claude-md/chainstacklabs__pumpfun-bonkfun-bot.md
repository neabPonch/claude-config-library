---
name: chainstacklabs__pumpfun-bonkfun-bot
source: https://github.com/chainstacklabs/pumpfun-bonkfun-bot/blob/9ab686b453fe5d2f1023fdcf46484b24d4c40f54/CLAUDE.md
repo: chainstacklabs/pumpfun-bonkfun-bot
kind: claude-md
stars: 956
last_pushed: 2026-05-19T20:03:02Z
license: apache-2.0
score: 9
domains: [blockchain, cli-tools, trading-bots]
tags: [solana, python, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# chainstacklabs/pumpfun-bonkfun-bot — claude-md

**Why it's worth keeping:** The 'Protocol notes' section provides critical low-level details like byte offsets and account counts to prevent LLM hallucinations regarding incomplete IDLs; the 'Learning Examples' provide actionable command templates for testing.

**Summary:** A high-density development guide for a Solana trading bot that includes specific build commands and deep technical protocol gotchas.

**Source credibility:** High credibility with 956 stars and recent activity (1 month ago).

**Recency:** Very current; reflects recent on-chain protocol upgrades.

**Source:** [chainstacklabs/pumpfun-bonkfun-bot/CLAUDE.md](https://github.com/chainstacklabs/pumpfun-bonkfun-bot/blob/9ab686b453fe5d2f1023fdcf46484b24d4c40f54/CLAUDE.md) · 956★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pump Bot Development Guide

This is a trading bot for pump.fun and letsbonk.fun platforms that snipes new tokens and implements various trading strategies.

## Project Structure

- `src/` - Main source code
- `learning-examples/` - Educational scripts and examples
- `bots/` - Bot configuration files (YAML)
- `logs/` - Log files from bot executions
- `idl/` - Interface definition files for Solana programs

## Bash Commands & Development

### Setup Commands
```bash
# Install dependencies
uv sync

# Activate virtual environment (Unix/macOS)
source .venv/bin/activate

# Install as editable package
uv pip install -e .
```

### Running the Bot
```bash
# Run as installed package
pump_bot

# Run directly
uv run src/bot_runner.py
```

### Learning Examples
```bash
# Bonding curve status
uv run learning-examples/bonding-curve-progress/get_bonding_curve_status.py TOKEN_ADDRESS

# Listen to migrations
uv run learning-examples/listen-migrations/listen_logsubscribe.py
uv run learning-examples/listen-migrations/listen_blocksubscribe_old_raydium.py

# Compute associated bonding curve
uv run learning-examples/compute_associated_bonding_curve.py

# Listen to new tokens
uv run learning-examples/lis
```

</details>
