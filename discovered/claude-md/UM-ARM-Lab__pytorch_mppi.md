---
name: UM-ARM-Lab__pytorch_mppi
source: https://github.com/UM-ARM-Lab/pytorch_mppi/blob/e04a569cd4215e705f9013145c496fc59cb25ed6/CLAUDE.md
repo: UM-ARM-Lab/pytorch_mppi
kind: claude-md
stars: 716
last_pushed: 2026-03-15T09:20:04Z
license: mit
score: 9
domains: [robotics, machine-learning, performance-optimization]
tags: [pytorch, mppi, high-performance, vectorization]
curated: 2026-06-15
curated_by: config-scout
---

# UM-ARM-Lab/pytorch_mppi — claude-md

**Why it's worth keeping:** It identifies exact code patterns that cause graph breaks (e.g., list appends) and provides a granular roadmap for optimization rather than just describing the API.

**Summary:** Provides high-density technical intelligence regarding performance bottlenecks, torch.compile blockers, and specific vectorization strategies.

**Source credibility:** High-quality research repo from UM-ARM-Lab with significant stars and recent maintenance.

**Recency:** Very current; explicitly addresses modern PyTorch workflows like torch.compile and vmap migration.

**Source:** [UM-ARM-Lab/pytorch_mppi/CLAUDE.md](https://github.com/UM-ARM-Lab/pytorch_mppi/blob/e04a569cd4215e705f9013145c496fc59cb25ed6/CLAUDE.md) · 716★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# pytorch_mppi

Model Predictive Path Integral (MPPI) control library using approximate dynamics in PyTorch.
Implements batched trajectory sampling for GPU-accelerated model-based control.

## Project Structure

```
src/pytorch_mppi/
  __init__.py          # Exports MPPI, SMPPI, KMPPI
  mppi.py              # Core implementation (~625 lines): MPPI, SMPPI, KMPPI, run_mppi
  autotune.py          # Hyperparameter tuning infrastructure (CMA-ES local optimizer)
  autotune_global.py   # Ray Tune global search integration
  autotune_qd.py       # Quality Diversity optimization (CMA-ME via pyribs)
tests/
  pendulum.py                       # MPPI on true pendulum dynamics (gym)
  pendulum_approximate.py           # MPPI with learned neural network dynamics
  pendulum_approximate_continuous.py # Continuous angle representation variant
  smooth_mppi.py                    # Visual comparison of MPPI, SMPPI, KMPPI
  auto_tune_parameters.py           # Hyperparameter tuning example
  test_batch_wrapper.py             # Unit tests for handle_batch_input
```

## Architecture

### Class Hierarchy
- **MPPI** - Base class. Batched trajectory sampling with importance-weighted control update (Algorith
```

</details>
