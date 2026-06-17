---
name: disciplinedware__swiftward-ai-trading-agents__claude
source: https://github.com/disciplinedware/swiftward-ai-trading-agents/blob/d02e4e6de9f4df917ddcc75ae32e1484428fa840/ruby/agents/solid_loop_trading/CLAUDE.md
repo: disciplinedware/swiftward-ai-trading-agents
kind: claude-md
stars: 3
last_pushed: 2026-04-12T07:22:00Z
license: mit
score: 9
domains: [backend, agents-ai, ruby-on-rails]
tags: [debugging-snippets, model-mapping, docker-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# disciplinedware/swiftward-ai-trading-agents — claude-md

**Why it's worth keeping:** Includes highly actionable 'rails runner' debugging snippets that allow an LLM to inspect state inside Docker containers without manual DB access; also maps model relationships clearly to prevent schema hallucinations.

**Summary:** Provides structural mapping of a Rails-based trading agent and specific instructions for navigating domain models and dependencies.

**Source credibility:** Niche, specialized trading project with recent activity.

**Recency:** Very current; perfectly optimized for agentic terminal-based workflows.

**Source:** [disciplinedware/swiftward-ai-trading-agents/ruby/agents/solid_loop_trading/CLAUDE.md](https://github.com/disciplinedware/swiftward-ai-trading-agents/blob/d02e4e6de9f4df917ddcc75ae32e1484428fa840/ruby/agents/solid_loop_trading/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Solid Loop Trading — Ruby Rails Agent

Ruby/Rails backtesting and swarm agent. Runs at http://localhost:7175.
App code: `ruby/agents/solid_loop_trading/` (this directory, inside ai-trading-agents repo).

**SolidLoop gem** (framework): https://github.com/Ruslan/solid_loop
To study the gem source, clone it into a temp folder:
```bash
git clone https://github.com/Ruslan/solid_loop /tmp/solid_loop
```
Do not edit it in place — treat as read-only reference.

## Code layout

| What | Path |
|------|------|
| Models | `app/models/` |
| Agents | `app/agents/` |
| MCP tools | `app/services/mcp_tools/` |
| PnL presenter | `app/presenters/local_trading_session_presenter.rb` |
| DB migrations | `db/migrate/` |

## Key models

- **AgentRun** — one agent execution. Has `loop` (SolidLoop::Loop), no direct `pnl` field.
- **SolidLoop::Loop** — agent loop: `state` (JSONB), `cost`, `step_count`, `messages`.
- **TradingSession** — virtual trading env with ledger. Often 0 rows (sessions managed via MCP).
- **LedgerEntry** — accounting (trade/fill/reservation/deposit). Source of truth for equity.
- **LocalTradingSessionPresenter** — computes `initial_balance`, `total_equity_usdt`, `ledger_rows`.

## D
```

</details>
