---
name: rschaeff__dpam_c2
source: https://github.com/rschaeff/dpam_c2/blob/31fe01b59d9191d561f78af37b591bdba947658c/CLAUDE.md
repo: rschaeff/dpam_c2
kind: claude-md
stars: 1
last_pushed: 2026-05-03T06:36:12Z
license: unknown
score: 9
domains: [bioinformatics, cli-tools, hpc]
tags: [slurm, python, batch-processing, scientific-computing]
curated: 2026-06-15
curated_by: config-scout
---

# rschaeff/dpam_c2 — claude-md

**Why it's worth keeping:** Includes 'CRITICAL' warnings about I/O bottlenecks and environment footguns like OMP_PROC_BIND. Provides production-ready shell templates that solve complex environment and performance issues.

**Summary:** A highly specialized guide for running a bioinformatics pipeline on High-Performance Computing (HPC) clusters using SLURM.

**Source credibility:** High; the content demonstrates expert knowledge of specific high-performance computing infrastructure constraints.

**Recency:** Very recent (1 month ago), highly relevant to modern dev/ops workflows.

**Source:** [rschaeff/dpam_c2/CLAUDE.md](https://github.com/rschaeff/dpam_c2/blob/31fe01b59d9191d561f78af37b591bdba947658c/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DPAM v2.0 is a modern Python 3 reimplementation of the Domain Parser for AlphaFold Models. It identifies structural domains through a 24-step pipeline integrating sequence homology (HHsearch), structural similarity (Foldseek, DALI), geometric analysis, confidence metrics (pLDDT, PAE), and machine learning (DOMASS/TensorFlow) for ECOD classification.

## Development Setup

```bash
# Install package in development mode
pip install -e . --break-system-packages

# With development dependencies (testing, type checking, formatting)
pip install -e ".[dev]" --break-system-packages

# Run tests
pytest tests/                    # All tests
pytest tests/unit/               # Unit tests only (fast, no external deps)
pytest tests/integration/        # Integration tests (require external tools)
pytest -m "not slow"             # Skip slow tests
pytest tests/integration/test_step02_hhsearch.py::TestStep02HHsearch::test_hhsearch_basic  # Single test

# With coverage
pytest --cov=dpam tests/

# Type checking
mypy dpam/

# Code formatting
black dpam/
flake8 dpam/
```

</details>
