---
name: studiogangster__next-gen-algo-trading-bot__skill
source: https://github.com/studiogangster/next-gen-algo-trading-bot/blob/2565dce5b9fb0125c4fc6a9117cdc4bc768223bc/skills/ngat-dashboard/SKILL.md
repo: studiogangster/next-gen-algo-trading-bot
kind: skill
stars: 35
last_pushed: 2026-05-11T07:42:19Z
license: unknown
score: 7
domains: [data-visualization, algorithmic-trading, observability]
tags: [streamlit, dash, parquet, diagnostics]
curated: 2026-06-15
curated_by: config-scout
---

# studiogangster/next-gen-algo-trading-bot — skill

**Why it's worth keeping:** The inclusion of 'Cons' and 'Caveats' is excellent; it proactively warns the agent about technical debt, timezone risks, and performance bottlenecks.

**Summary:** Provides instructions for maintaining local observability dashboards via Streamlit and Dash using parquet-backed data.

**Source credibility:** Niche project with modest star count (35) and active maintenance history.

**Recency:** Very recent; updated within the last month.

**Source:** [studiogangster/next-gen-algo-trading-bot/skills/ngat-dashboard/SKILL.md](https://github.com/studiogangster/next-gen-algo-trading-bot/blob/2565dce5b9fb0125c4fc6a9117cdc4bc768223bc/skills/ngat-dashboard/SKILL.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ngat-dashboard
description: Maintain local operator dashboards in dashboard/ using Streamlit and Dash for candle inspection and indicator visualization. Use when improving manual observability, chart behavior, or live diagnostics from parquet-backed data.
---

# Ngat Dashboard

## Overview

Support quick local introspection tools for candles and indicators separate from the production-facing Vue dashboard.

## Submodules

- `dashboard/visualize.py`: Streamlit dashboard with candle/Keltner rendering.
- `dashboard/dash_app.py`: Dash dashboard with symbol/timeframe selection and overlays.

## Pros

- Keep immediate visual feedback while debugging aggregation paths.
- Keep no dependency on frontend build chain for basic diagnostics.

## Cons

- Maintain two dashboard stacks (Streamlit + Dash) with duplicated logic.
- Tie to local parquet files instead of Redis/API source of truth.

## Caveats

- Guard timezone conversions; some files assume timezone-aware timestamps.
- Keep timeframe support consistent; `day` and higher frames are partially handled.
- Watch performance for full-file parquet reads on each refresh.

## Forward Features

- Add shared chart utility module reused
```

</details>
