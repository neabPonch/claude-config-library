---
name: HFooladi__molax
source: https://github.com/HFooladi/molax/blob/9d5a79bc0daae15fc6d0b6cc7d2ffa6ef7f6498c/CLAUDE.md
repo: HFooladi/molax
kind: claude-md
stars: 1
last_pushed: 2026-04-30T13:06:19Z
license: mit
score: 9
domains: [machine-learning, data-science]
tags: [jax, active-learning, high-performance]
curated: 2026-06-15
curated_by: config-scout
---

# HFooladi/molax — claude-md

**Why it's worth keeping:** The 'Performance-Critical Pattern' section includes a vital 'Good vs Bad' code comparison specific to the framework's performance traps, alongside a clear API contract for structural consistency.

**Summary:** This config provides essential high-performance JAX patterns to prevent costly JIT recompilation and defines a consistent architectural pattern for all model implementations.

**Source credibility:** Niche research repository with recent maintenance activity.

**Recency:** Current; utilizes modern Flax 0.11+ and JAX patterns.

**Source:** [HFooladi/molax/CLAUDE.md](https://github.com/HFooladi/molax/blob/9d5a79bc0daae15fc6d0b6cc7d2ffa6ef7f6498c/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code when working with this repository.

## Project Overview

Molax is a high-performance JAX framework for molecular active learning. It uses **jraph** for efficient graph batching, achieving ~400x speedup over naive implementations.

## Quick Commands

```bash
# Setup (using uv)
source setup.sh

# Test
pytest tests/

# Format and lint (ruff for both)
ruff format .
ruff check .

# Build docs locally
uv pip install -e .[docs]
mkdocs serve

# Run examples
python examples/simple_active_learning.py
python examples/active_learning_benchmark.py
python examples/mpnn_demo.py
python examples/gat_demo.py
python examples/graph_transformer_demo.py
python examples/ensemble_active_learning.py
python examples/evidential_active_learning.py
python examples/acquisition_strategies_demo.py
python examples/calibration_comparison.py
python examples/uncertainty_gcn_demo.py
```

## Architecture

### Performance-Critical Pattern

**IMPORTANT**: The key to performance is batching all data once and using masking:

```python
# GOOD - batch once, use masking (fast)
all_graphs = jraph.batch(train_data.graphs)
labeled_mask = jnp.zeros(n_train, dtype=bool).at[labeled_indices].set
```

</details>
