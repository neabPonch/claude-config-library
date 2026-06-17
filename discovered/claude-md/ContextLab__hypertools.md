---
name: ContextLab__hypertools
source: https://github.com/ContextLab/hypertools/blob/125a09b556c080e5d8bd464154116da2a7f0c044/CLAUDE.md
repo: ContextLab/hypertools
kind: claude-md
stars: 1882
last_pushed: 2026-01-29T06:12:28Z
license: mit
score: 8
domains: [data-science, mathematical-computing, python-library]
tags: [architecture-map, workflow-logic, functional-programming]
curated: 2026-06-15
curated_by: config-scout
---

# ContextLab/hypertools — claude-md

**Why it's worth keeping:** The 'Data Flow' section and the detailed mapping of modules/functions provide a mental model that prevents Claude from getting lost in large directories.

**Summary:** Provides an excellent structural map of the library by linking high-level functions to their specific file locations and defining the data transformation pipeline.

**Source credibility:** High: a well-starred (1.8k) specialized scientific library with recent maintenance.

**Recency:** 

**Source:** [ContextLab/hypertools/CLAUDE.md](https://github.com/ContextLab/hypertools/blob/125a09b556c080e5d8bd464154116da2a7f0c044/CLAUDE.md) · 1882★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HyperTools is a Python library for visualizing and manipulating high-dimensional data. It provides a unified interface for dimensionality reduction, data alignment, clustering, and visualization, built on top of matplotlib, scikit-learn, and seaborn.

## Key Commands

### Testing
- `pytest` - Run all tests from the hypertools/ directory
- `pytest tests/test_<module>.py` - Run tests for a specific module
- `pytest tests/test_<module>.py::test_<function>` - Run a specific test function

### Development Setup
- `pip install -e .` - Install in development mode
- `pip install -r requirements.txt` - Install dependencies
- `pip install -r docs/doc_requirements.txt` - Install documentation dependencies

### Documentation
- `cd docs && make html` - Build HTML documentation
- `cd docs && make clean` - Clean documentation build files

## Code Architecture

### Core Components

**DataGeometry Class** (`hypertools/datageometry.py`)
- Central data container that holds raw data, transformed data, and transformation parameters
- Stores matplotlib figure/axes han
```

</details>
