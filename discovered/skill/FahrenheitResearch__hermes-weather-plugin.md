---
name: FahrenheitResearch__hermes-weather-plugin
source: https://github.com/FahrenheitResearch/hermes-weather-plugin/blob/d474493ef4ffeefabad9dbf0188f72bce3b47b67/skill.md
repo: FahrenheitResearch/hermes-weather-plugin
kind: skill
stars: 33
last_pushed: 2026-04-05T01:30:52Z
license: unknown
score: 9
domains: [agents-ai, geospatial, weather-api]
tags: [tool-usage, optimization, weather]
curated: 2026-06-14
curated_by: config-scout
---

# FahrenheitResearch/hermes-weather-plugin — skill

**Why it's worth keeping:** It includes high-value patterns like tool sequencing (lightweight vs. heavy), batching multiple requests into one call, and converting qualitative regions into quantitative lat/lon/radius parameters.

**Summary:** A specialized instruction set that optimizes tool usage through efficiency heuristics and geospatial translation.

**Source credibility:** Solid niche project with active maintenance evidenced by a 2-month-old push.

**Recency:** Highly current; utilizes modern agentic optimization strategies.

**Source:** [FahrenheitResearch/hermes-weather-plugin/skill.md](https://github.com/FahrenheitResearch/hermes-weather-plugin/blob/d474493ef4ffeefabad9dbf0188f72bce3b47b67/skill.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: weather-plugin
description: Guide for using the weather plugin — data queries, radar imagery, model maps, and meteorological calculations
version: 2.0.0
metadata:
  hermes:
    tags: [weather, radar, forecast, meteorology]
    category: weather
---

# Weather Plugin Usage Guide

You have 12 weather tools. Prefer lightweight data tools and only use images when asked.

## Tool Selection

**"How's the weather in [place]?"** → `wx_conditions`
**"What's the forecast?"** → `wx_forecast`
**"Any warnings/watches?"** → `wx_alerts`
**"Show me the radar"** → `wx_radar_image`
**"Show me CAPE/temperature/wind map"** → `wx_model_image` (use comma-separated vars: `"cape,helicity,uh,srh"` for multiple in ONE call)
**"What's the severe weather outlook?"** → `wx_severe`
**"Weather in Tokyo/London/etc"** → `wx_global` (worldwide)
**"Calculate dewpoint/wind chill/LCL"** → `wx_calc`
**"Is there a tornado threat?"** → `wx_severe` first, then `wx_model_image --var cape` or `--var helicity` for visual
**"What does the HRRR show?"** → `wx_model_image` with appropriate var
**"Show me the 18z HRRR"** → `wx_model_image` with `cycle: 18`
**"Sounding at a point"** → `wx_sounding`

## IMPORTANT: Only t
```

</details>
