---
name: marketcalls__openalgo
source: https://github.com/marketcalls/openalgo/blob/ee8b303f99477563c2bbe94a455d7d586444f5f8/CLAUDE.md
repo: marketcalls/openalgo
kind: claude-md
stars: 2043
last_pushed: 2026-06-15T01:50:24Z
license: agpl-3.0
score: 9
domains: [fintech, backend-api, trading-systems, python]
tags: [architectural-patterns, concurrency-warnings, instructional]
curated: 2026-06-15
curated_by: config-scout
---

# marketcalls/openalgo — claude-md

**Why it's worth keeping:** Contains critical 'gotcha' warnings (like the SQLite NullPool necessity) and provides clear structural templates for new broker integrations to ensure consistency.

**Summary:** Provides deep architectural insights into a complex trading system, covering database concurrency pitfalls, WebSocket pipelines, and specific toolchain requirements.

**Source credibility:** High; an active project with significant stars and highly detailed technical documentation.

**Recency:** Very current, referencing React 19, Python 3.12, and upcoming regulatory mandates.

**Source:** [marketcalls/openalgo/CLAUDE.md](https://github.com/marketcalls/openalgo/blob/ee8b303f99477563c2bbe94a455d7d586444f5f8/CLAUDE.md) · 2043★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

OpenAlgo is a production-ready algorithmic trading platform built with Flask (backend) and React 19 (frontend). It is **four products in one self-hosted instance**, all sharing a single broker session and WebSocket feed:

| Surface | Route | Purpose |
| --- | --- | --- |
| **Unified Broker API** | `/api/v1/` | External platforms (TradingView, Amibroker, ChartInk, Excel, Python, MCP) |
| **Python Strategy Host** | `/python` | In-browser CodeMirror editor — paste scripts, schedule on IST times, run parallel strategies with process isolation and live logs |
| **Flow (No-Code Builder)** | `/flow` | Drag-and-drop nodes: market data → indicators → conditions → order execution; JSON import/export |
| **Options Trading Suite** | `/tools` | 12 analytical tools: Strategy Builder, Option Chain, IV Smile, Max Pain, Vol Surface, GEX, OI Tracker, Straddle Chart, etc. |

All surfaces share the Sandbox engine (₹1 Crore sandbox capital, exchange-aligned auto square-off) and support Telegram alerts.

**Repository**: https://github.com/marketcalls/openalgo
**Documentation*
```

</details>
