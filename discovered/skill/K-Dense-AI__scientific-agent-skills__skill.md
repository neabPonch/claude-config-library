---
name: K-Dense-AI__scientific-agent-skills__skill
source: https://github.com/K-Dense-AI/scientific-agent-skills/blob/2b4cce7d8763232864fa3dff701e311636bcc62f/skills/statsmodels/SKILL.md
repo: K-Dense-AI/scientific-agent-skills
kind: skill
stars: 28254
last_pushed: 2026-06-13T14:30:30Z
license: mit
score: 9
domains: [data-science, statistics, python]
tags: [regression, time-series, econometrics, diagnostics]
curated: 2026-06-15
curated_by: config-scout
---

# K-Dense-AI/scientific-agent-skills — skill

**Why it's worth keeping:** Includes critical diagnostic steps (e.g., ADF tests, heteroskedasticity checks) that guide the agent through validation logic rather than just syntax. It also highlights essential boilerplate like `sm.add_constant` which prevents common modeling errors.

**Summary:** Provides highly structured, procedure-oriented instructions for statistical modeling, including regression, time series, and GLM workflows.

**Source credibility:** Extremely high; the repository has significant social proof (28k+ stars) and is specialized for scientific agents.

**Recency:** Current; utilizes modern Python tooling like `uv` and up-to-date library versions.

**Source:** [K-Dense-AI/scientific-agent-skills/skills/statsmodels/SKILL.md](https://github.com/K-Dense-AI/scientific-agent-skills/blob/2b4cce7d8763232864fa3dff701e311636bcc62f/skills/statsmodels/SKILL.md) · 28254★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: statsmodels
description: Statistical models library for Python. Use when you need specific model classes (OLS, GLM, mixed models, ARIMA) with detailed diagnostics, residuals, and inference. Best for econometrics, time series, rigorous inference with coefficient tables. For guided statistical test selection with APA reporting use statistical-analysis.
allowed-tools: Read Write Edit Bash
compatibility: Requires Python 3.9+ and statsmodels 0.14.6-compatible dependencies. Use `uv pip install statsmodels==0.14.6`; optional predictive-metric examples also need scikit-learn.
license: BSD-3-Clause license
metadata: {"version": "1.1", "skill-author": "K-Dense Inc."}
---

# Statsmodels: Statistical Modeling and Econometrics

## Overview

Statsmodels is Python's premier library for statistical modeling, providing tools for estimation, inference, and diagnostics across a wide range of statistical methods. Apply this skill for rigorous statistical analysis, from simple linear regression to complex time series models and econometric analyses.

## Current Compatibility

Examples target statsmodels 0.14.6, released Dec 5, 2025. For reproducible environments, pin the primary package:

```
```

</details>
