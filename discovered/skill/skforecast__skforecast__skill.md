---
name: skforecast__skforecast__skill
source: https://github.com/skforecast/skforecast/blob/397e2dc88e5bd3538011f72c0e79e8c4b132959c/skills/drift-detection/SKILL.md
repo: skforecast/skforecast
kind: skill
stars: 1503
last_pushed: 2026-06-15T17:46:19Z
license: bsd-3-clause
score: 9
domains: [data-science, machine-learning, mlops]
tags: [drift-detection, time-series, monitoring]
curated: 2026-06-16
curated_by: config-scout
---

# skforecast/skforecast — skill

**Why it's worth keeping:** Includes a practical 'Production loop' integration pattern and a critical 'Common Mistakes' section that prevents logical errors like fitting on test data.

**Summary:** Provides structured implementation patterns for monitoring time series model reliability using range and population drift detection.

**Source credibility:** Highly credible; skforecast is a well-established, specialized library for time series forecasting.

**Recency:** Current; follows modern MLOps practices for model monitoring and observability.

**Source:** [skforecast/skforecast/skills/drift-detection/SKILL.md](https://github.com/skforecast/skforecast/blob/397e2dc88e5bd3538011f72c0e79e8c4b132959c/skills/drift-detection/SKILL.md) · 1503★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: drift-detection
description: >
  Detects data drift in time series forecasting pipelines using
  RangeDriftDetector and PopulationDriftDetector. Covers range-based
  out-of-range detection and statistical distribution tests.
  Use when the user wants to monitor model reliability in production.
---

# Drift Detection

## When to Use

Use drift detection to monitor whether new data falls outside the patterns seen during training. This helps decide when to retrain a model.

| Detector | Speed | Use Case |
|----------|-------|----------|
| `RangeDriftDetector` | Very fast | Real-time inference — checks if values are in training range |
| `PopulationDriftDetector` | Moderate | Batch monitoring — statistical tests for distribution shifts |

## RangeDriftDetector

Checks whether new observations fall within the ranges seen during training. Lightweight and suitable for real-time scoring.

> `fit()` accepts `series` and `exog` as a pandas Series, DataFrame, or dict
> (useful for multi-series pipelines with `ForecasterRecursiveMultiSeries`).

```python
from skforecast.drift_detection import RangeDriftDetector
from skforecast.recursive import ForecasterRecursive

# 1. Train the fore
```

</details>
