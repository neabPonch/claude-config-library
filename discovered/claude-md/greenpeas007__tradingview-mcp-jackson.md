---
name: greenpeas007__tradingview-mcp-jackson
source: https://github.com/greenpeas007/tradingview-mcp-jackson/blob/f62c3430f6e2643272b31b67c89c81b3ae232b97/CLAUDE.md
repo: greenpeas007/tradingview-mcp-jackson
kind: claude-md
stars: 36
last_pushed: 2026-04-07T16:37:37Z
license: other
score: 9
domains: [trading, automation, agent-orchestration, mcp]
tags: [decision-trees, context-management, tool-usage]
curated: 2026-06-16
curated_by: config-scout
---

# greenpeas007/tradingview-mcp-jackson — claude-md

**Why it's worth keeping:** The 'Decision Tree' workflow patterns and proactive 'Context Management Rules' (using summaries/filters) are elite-tier techniques for managing large tool outputs in agentic workflows.

**Summary:** Provides a highly structured decision tree for tool orchestration and strict context management protocols to prevent token bloat.

**Source credibility:** Solid; 36 stars indicates a useful niche tool with recent activity.

**Recency:** Highly relevant to current Claude Code capabilities regarding context window efficiency.

**Source:** [greenpeas007/tradingview-mcp-jackson/CLAUDE.md](https://github.com/greenpeas007/tradingview-mcp-jackson/blob/f62c3430f6e2643272b31b67c89c81b3ae232b97/CLAUDE.md) · 36★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TradingView MCP — Claude Instructions

68 tools for reading and controlling a live TradingView Desktop chart via CDP (port 9222).

## Decision Tree — Which Tool When

### "What's on my chart right now?"
1. `chart_get_state` → symbol, timeframe, chart type, list of all indicators with entity IDs
2. `data_get_study_values` → current numeric values from all visible indicators (RSI, MACD, BBands, EMAs, etc.)
3. `quote_get` → real-time price, OHLC, volume for current symbol

### "What levels/lines/labels are showing?"
Custom Pine indicators draw with `line.new()`, `label.new()`, `table.new()`, `box.new()`. These are invisible to normal data tools. Use:

1. `data_get_pine_lines` → horizontal price levels drawn by indicators (deduplicated, sorted high→low)
2. `data_get_pine_labels` → text annotations with prices (e.g., "PDH 24550", "Bias Long ✓")
3. `data_get_pine_tables` → table data formatted as rows (e.g., session stats, analytics dashboards)
4. `data_get_pine_boxes` → price zones / ranges as {high, low} pairs

Use `study_filter` parameter to target a specific indicator by name substring (e.g., `study_filter: "Profiler"`).

### "Give me price data"
- `data_get_ohlcv` with `summary: t
```

</details>
