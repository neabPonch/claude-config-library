---
name: x402agent__SolanaOS__skill
source: https://github.com/x402agent/SolanaOS/blob/37041b5d74e4da89b4f23b688588953911547651/docs/docs-site/public/skill.md
repo: x402agent/SolanaOS
kind: skill
stars: 9
last_pushed: 2026-06-13T01:27:41Z
license: mit
score: 8
domains: [cli-tools, system-automation, trading-bots]
tags: [deployment-guide, daemonization, one-shot-prompt]
curated: 2026-06-15
curated_by: config-scout
---

# x402agent/SolanaOS — skill

**Why it's worth keeping:** Features a highly effective 'One-Shot Agent Prompt' for orchestration; includes explicit post-installation verification steps (curl/status) to ensure success.

**Summary:** A high-fidelity deployment manual that guides an agent through the full lifecycle of a complex system, including daemonization and hardware integration.

**Source credibility:** Professional-grade project with detailed systems programming documentation (Go, systemd, LaunchAgent).

**Recency:** Very current, reflecting modern local-first AI and agentic automation patterns.

**Source:** [x402agent/SolanaOS/docs/docs-site/public/skill.md](https://github.com/x402agent/SolanaOS/blob/37041b5d74e4da89b4f23b688588953911547651/docs/docs-site/public/skill.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SolanaOS — Agent Skill Sheet

> Give this file to any AI agent (Claude, Codex, GPT-4, MiniMax, etc.) to fully install, configure, and run SolanaOS in one shot.

---

## What You Are Installing

**SolanaOS Companion** — an autonomous Solana trading agent by SolanaOS Labs.

- Single ~10MB Go binary (`solanaos`)
- Runs a full OODA trading loop (RSI + EMA + ATR strategy)
- Telegram bot with live strategy controls
- Chrome extension with wallet + miner card
- Bitaxe Gamma 602 Bitcoin miner integration
- x402 payment protocol for monetized APIs
- macOS menu bar app + persistent LaunchAgent daemon
- Powered by a local-first Ollama harness (default: `minimax-m2.7:cloud`)

---

## Prerequisites

The agent should verify these exist before proceeding:

- `go` >= 1.21 (`go version`)
- `git` (`git --version`)
- `curl` (`curl --version`)
- macOS (for LaunchAgent) or Linux (for systemd)
- A `.env` file in the project root (see Step 2)

---

## Step 1 — Clone the Repo

```bash
git clone https://github.com/x402agent/SolanaOS solanaos
cd solanaos
```

---

## Step 2 — Create `.env`

Create a `.env` file in the project root. Minimum required fields:

```bash
# ── Required ──────────────────────────
```

</details>
