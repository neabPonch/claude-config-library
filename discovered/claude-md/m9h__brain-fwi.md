---
name: m9h__brain-fwi
source: https://github.com/m9h/brain-fwi/blob/b62c98eef1bfe83c26ccfc303ebb0afd586ee3b7/CLAUDE.md
repo: m9h/brain-fwi
kind: claude-md
stars: 0
last_pushed: 2026-05-09T15:58:36Z
license: unknown
score: 8
domains: [scientific-computing, physics-simulation, machine-learning]
tags: [jax, wave-inversion, scientific-python, uv]
curated: 2026-06-15
curated_by: config-scout
---

# m9h/brain-fwi — claude-md

**Why it's worth keeping:** Includes critical domain knowledge like SI units/grid spacing requirements and specific environmental nuances like Apple Silicon GPU sidecars and 'uv' package management.

**Summary:** A high-quality technical guide for a JAX-based scientific simulation project that defines physics constraints and environment rules.

**Source credibility:** Specialized scientific codebase, though currently a small-scale solo project.

**Recency:** Very current; uses modern tools like `uv` and JAX.

**Source:** [m9h/brain-fwi/CLAUDE.md](https://github.com/m9h/brain-fwi/blob/b62c98eef1bfe83c26ccfc303ebb0afd586ee3b7/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Brain FWI

## What is this project?

**brain-fwi** is a JAX-based Full Waveform Inversion (FWI) pipeline for
transcranial ultrasound brain imaging. It uses j-Wave's pseudospectral
solver for forward simulation and JAX autodiff for gradient computation,
following the approach of Guasch et al. (2020, npj Digital Medicine) but
reimplemented in a fully differentiable JAX framework.

Key innovation: replaces Stride/Devito adjoint-state gradients with
JAX automatic differentiation through j-Wave, enabling easy integration
with neural posterior estimation (SBI) and modern optimization.

## Architecture

```
brain_fwi/
  phantoms/       # Head model loading (BrainWeb, MIDA) + acoustic properties
  transducers/    # Ultrasound array geometry (ring, helmet)
  simulation/     # j-Wave forward solver wrapper
  inversion/      # FWI loop (losses, optimizer, multi-frequency)
  utils/          # Source wavelets, visualization helpers
```

## Key dependencies

| Library | Role |
|---------|------|
| j-Wave  | Pseudospectral acoustic wave solver (JAX) |
| jaxdf   | Domain/field discretization for j-Wave |
| JAX     | Autodiff + GPU acceleration |
| Equinox | Pytree-compatible modules
```

</details>
