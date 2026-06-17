---
name: zsylvester__meanderpy
source: https://github.com/zsylvester/meanderpy/blob/0b836b4896ced7e70aab6d81972d81bc72e86d57/CLAUDE.md
repo: zsylvester/meanderpy
kind: claude-md
stars: 163
last_pushed: 2026-02-13T10:33:41Z
license: apache-2.0
score: 9
domains: [scientific-computing, python, simulation]
tags: [physics-engine, numerical-methods, parameter-reference]
curated: 2026-06-14
curated_by: config-scout
---

# zsylvester/meanderpy — claude-md

**Why it's worth keeping:** The 'Key Parameters' table provides essential context for simulation tuning, while the 'Numerical Stability' section offers proactive troubleshooting advice for mathematical edge cases.

**Summary:** Provides deep domain-specific logic (CFL stability) alongside structure and typical usage patterns.

**Source credibility:** High-quality research project with clear ownership and niche popularity.

**Recency:** Very recent; fully compatible with modern LLM-assisted development.

**Source:** [zsylvester/meanderpy/CLAUDE.md](https://github.com/zsylvester/meanderpy/blob/0b836b4896ced7e70aab6d81972d81bc72e86d57/CLAUDE.md) · 163★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Meanderpy Project Guide

## Project Overview

Meanderpy is a Python library implementing a numerical model of meandering rivers based on the Howard & Knutson (1984) kinematic approach. It simulates channel migration, cutoff formation, and builds 3D stratigraphic models from centerline evolution.

**Author**: Zoltan Sylvester (zoltan.sylvester@beg.utexas.edu)
**Version**: 0.2.0
**License**: Apache 2.0

## Quick Commands

```bash
# Install in development mode
pip install -e .

# Run Jupyter notebooks
jupyter lab meanderpy/meanderpy.ipynb

# Create conda environment
conda env create -f environment.yml
```

## Project Structure

```
meanderpy/
├── meanderpy/
│   ├── __init__.py          # Package init
│   ├── meanderpy.py         # Core module (~1750 lines)
│   └── *.ipynb              # Example notebooks
├── setup.py                 # Package configuration
└── environment.yml          # Conda environment
```

## Core Architecture

### Main Classes (meanderpy.py)

- **`Channel`** - Single channel centerline (x, y, z coords, W width, D depth)
- **`Cutoff`** - Oxbow lake/abandoned loop representation
- **`ChannelBelt`** - Collection of channels over time; main simulation co
```

</details>
