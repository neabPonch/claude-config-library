---
name: rsnemmen__nmmn
source: https://github.com/rsnemmen/nmmn/blob/a23ea3d8d286171f84fe727a22fd19371ea6b9cd/CLAUDE.md
repo: rsnemmen/nmmn
kind: claude-md
stars: 27
last_pushed: 2026-05-05T21:57:29Z
license: mit
score: 7
domains: [scientific-computing, python]
tags: [astronomy, architecture-map, module-overview]
curated: 2026-06-15
curated_by: config-scout
---

# rsnemmen/nmmn — claude-md

**Why it's worth keeping:** The Module Architecture table and dependency groupings allow an agent to navigate complex domain logic without scanning every file.

**Summary:** Provides a structured map of scientific modules and clear build/install workflows.

**Source credibility:** A specialized scientific repository with active maintenance.

**Recency:** Current; explicitly mentions Claude Code instructions.

**Source:** [rsnemmen/nmmn/CLAUDE.md](https://github.com/rsnemmen/nmmn/blob/a23ea3d8d286171f84fe727a22fd19371ea6b9cd/CLAUDE.md) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**nmmn** is a miscellaneous scientific computing Python library for astronomy, data analysis, signal processing, and numerical simulations by Rodrigo Nemmen. Published on PyPI as `nmmn`.

## Development Setup

```bash
# Development install (edits take effect immediately)
pip install -e .

# Regular install
pip install .
```

## Building and Publishing

```bash
# Build distribution
python -m build

# Upload to PyPI
twine upload dist/*
```

## Documentation

```bash
# Build Sphinx docs
cd docs && make html
```

## Module Architecture

All modules live in `nmmn/`:

| Module | Purpose |
|--------|---------|
| `astro.py` | Redshift/distance conversions, flux unit conversions, physical constants (CGS) |
| `lsd.py` | Array/list/set operations: NaN removal (`delnan`), set operations, bootstrapping, normalization |
| `dsp.py` | Digital signal processing: peak detection, smoothing, Lomb-Scargle periodogram, wavelet transforms |
| `stats.py` | Statistics: scatter, confidence/prediction bands, goodness-of-fit, p-values |
| `bayes.py` | Bayesian statistics: p
```

</details>
