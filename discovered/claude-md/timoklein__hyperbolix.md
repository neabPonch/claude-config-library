---
name: timoklein__hyperbolix
source: https://github.com/timoklein/hyperbolix/blob/448145881539c360640ee61a37cc09bc9acb702f/CLAUDE.md
repo: timoklein/hyperbolix
kind: claude-md
stars: 6
last_pushed: 2026-06-12T14:45:31Z
license: mit
score: 9
domains: [machine-learning, scientific-computing]
tags: [jax, flax, numerical-stability, deep-learning]
curated: 2026-06-16
curated_by: config-scout
---

# timoklein/hyperbolix — claude-md

**Why it's worth keeping:** Includes 'numerical gotchas' like specific weight initialization rules and float precision warnings that prevent silent mathematical errors. It also enforces highly specific coding standards like dimension suffixing and version-specific API patterns.

**Summary:** Provides deep architectural context and mathematical constraints for a high-performance JAX/Flax library. It acts as both a developer manual and a numerical stability guide.

**Source credibility:** The source is a specialized, active research repository for hyperbolic deep learning.

**Recency:** 

**Source:** [timoklein/hyperbolix/CLAUDE.md](https://github.com/timoklein/hyperbolix/blob/448145881539c360640ee61a37cc09bc9acb702f/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Quick Reference Commands

```bash
# Install
uv sync --locked --dev

# Run all tests (~1,660 tests)
uv run pytest

# Run a single test file
uv run pytest tests/test_manifolds.py -v

# Run a single test function
uv run pytest tests/test_manifolds.py::test_dist -v

# Run a fast subset (dim2 only)
uv run pytest -k "dim2"

# Lint and format
uv run ruff check hyperbolix tests benchmarks
uv run ruff format hyperbolix tests benchmarks

# Type check
uv run pyright hyperbolix

# All pre-commit hooks
uv run pre-commit run --all-files

# Benchmarks
uv run pytest benchmarks/ --benchmark-only

# Docs
uv run mkdocs serve
uv run mkdocs build --strict
```

## Verification

After making changes, run the test files that cover the affected code:
```bash
uv run pytest tests/<relevant_test_file>.py -x -v
```
For example: manifold changes → `test_manifolds.py`, optimizer changes → `test_optimizers.py`, FGG layer changes → `nn_layers/test_hyperboloid_fgg.py`. Use `-k "dim2"` to speed up parametrized tests during iteration.

## Architecture

**hyperbolix** is a pure JAX library for hyperb
```

</details>
