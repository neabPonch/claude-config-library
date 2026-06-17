---
name: secutils-dev__secutils__forecast-skill
source: https://github.com/secutils-dev/secutils/blob/c6d178a7ff39190824c12c67108d4d93c5e6e059/dev/tools/forecast.skill.md
repo: secutils-dev/secutils
kind: skill
stars: 100
last_pushed: 2026-06-14T13:01:21Z
license: agpl-3.0
score: 9
domains: [data-science, visualization, forecasting, analytics]
tags: [time-series, statistics, deep-linking, data-analysis]
curated: 2026-06-15
curated_by: config-scout
---

# secutils-dev/secutils — skill

**Why it's worth keeping:** Uses advanced URL fragment/query parameter patterns to enable 'one-click' data preloading in an external UI. The trigger list is highly semantic, mapping natural language requests to specific statistical functions.

**Summary:** Provides a specialized skill for statistical time-series analysis, including trend fitting, anomaly detection, and backtesting via an external web tool.

**Source credibility:** High; comes from a specialized security/engineering toolbox with active maintenance and community validation.

**Recency:** Highly relevant for modern agentic workflows that offload complex computation to specialized web-based UIs.

**Source:** [secutils-dev/secutils/dev/tools/forecast.skill.md](https://github.com/secutils-dev/secutils/blob/c6d178a7ff39190824c12c67108d4d93c5e6e059/dev/tools/forecast.skill.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: forecast
description: >-
  Fit a trendline to numeric data, project N periods into the future, smooth
  noisy series, or hunt for anomalies using the Secutils.dev Forecast tool.
  Hand the user https://tools.secutils.dev/forecast (optionally with
  ?example=<id> to deep-link a curated dataset, or with the user's own data
  encoded in the URL fragment for one-click preload), tell them to pick a
  Fit / Smoothing / Forecast / Anomaly mode on the right and watch the
  chart update. Trigger when the user asks to "fit a trendline", "forecast
  the next N months", "find anomalies in this metric", "smooth this noisy
  series", "is this growth linear or exponential", "when will we hit X
  users", or anything that names secutils.dev/forecast.
---

# Forecast (Secutils.dev)

In-browser trend forecaster powered by [`micro-ml`](https://github.com/AdamPerlinski/micro-ml)
(WASM, ~56 KB gzipped on its own, fully self-contained in the page bundle).
Paste a numeric series, choose a fit / smoothing / forecast horizon /
anomaly mode, and read the chart + the structured results panel.

Five kinds of jobs the tool handles well:

1. **Trend fit + N-period forecast** -- pick `Fit = Auto (best R
```

</details>
