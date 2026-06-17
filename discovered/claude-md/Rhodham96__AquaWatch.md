---
name: Rhodham96__AquaWatch
source: https://github.com/Rhodham96/AquaWatch/blob/3e867866a92ca8dfa0f63f9d46781e93e1f82c6d/claude.md
repo: Rhodham96/AquaWatch
kind: claude-md
stars: 0
last_pushed: 2026-05-05T07:36:01Z
license: unknown
score: 9
domains: [geospatial, scientific-computing, data-pipeline]
tags: [remote-sensing, sentinel-2, python, geospatial-analysis]
curated: 2026-06-14
curated_by: config-scout
---

# Rhodham96/AquaWatch — claude-md

**Why it's worth keeping:** The 'Critical Gotchas' section provides indispensable non-obvious API quirks (trailing slashes, specific response keys) and scientific scaling/CRS details that prevent common geospatial bugs.

**Summary:** A high-density technical manual for a satellite imagery processing pipeline involving Sentinel-2 and S3 data.

**Source credibility:** Written by a specialized AI/ML engineer; high technical depth despite low repository popularity.

**Recency:** Very current (pushed 1 month ago).

**Source:** [Rhodham96/AquaWatch/claude.md](https://github.com/Rhodham96/AquaWatch/blob/3e867866a92ca8dfa0f63f9d46781e93e1f82c6d/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is AquaWatch
A satellite-based water quality monitoring prototype that detects cyanobacteria blooms,
turbidity anomalies, and chlorophyll-a spikes in drinking water reservoirs using ESA
Sentinel-2 imagery. Built by Robin Hamers (AI/ML Engineer at WEO, weo-water.com, Luxembourg).

**Pilot reservoir:** Lac de Serre-Ponçon, France (44.5553°N, 6.3522°E, ~28 km²).
Known bloom events: summers 2019, 2022, 2023, 2024.
Validation date range: 2023-04-01 to 2024-10-31.

**Second reservoir (Weekend 6):** Embalse de Entrepeñas, Spain (40.55°N, 2.69°W, ~80 km²).
Known bloom events: Jul–Sep 2022 and Jul–Sep 2023.
Validation date range: 2022-04-05 to 2023-10-18. Both bloom periods validated with no threshold retuning.

## Commands

```bash
# Activate environment (required before any command)
conda activate aquawatch

# Create environment from scratch
conda env create -f environment.yml

# Run the Weekend 1 integration test (search → download → mask → clip → preview)
python scripts/test_pipeline.py

# All scripts add src/ to sys.path via PROJECT_ROOT; run from repo root

# We
```

</details>
