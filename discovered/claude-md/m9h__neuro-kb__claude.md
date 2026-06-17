---
name: m9h__neuro-kb__claude
source: https://github.com/m9h/neuro-kb/blob/60a30d071adb875c9987b8ec9ef44b868b4c0fcb/raw/projects/brain-fwi/CLAUDE.md
repo: m9h/neuro-kb
kind: claude-md
stars: 0
last_pushed: 2026-06-13T17:15:21Z
license: unknown
score: 9
domains: [scientific-computing, physics]
tags: [jax, simulations, uv]
curated: 2026-06-15
curated_by: config-scout
---

# m9h/neuro-kb — claude-md

**Why it's worth keeping:** Includes critical scientific conventions (SI units, grid spacing rules) and strict tooling requirements (uv only) that prevent AI from making incorrect physical or environment assumptions.

**Summary:** Provides essential domain-specific constraints and architectural context for a JAX-based physics simulation project.

**Source credibility:** Highly specialized research code; appears to be a professional/academic implementation.

**Recency:** Very current, utilizing modern Python toolchains like uv and JAX-based ecosystems.

**Source:** [m9h/neuro-kb/raw/projects/brain-fwi/CLAUDE.md](https://github.com/m9h/neuro-kb/blob/60a30d071adb875c9987b8ec9ef44b868b4c0fcb/raw/projects/brain-fwi/CLAUDE.md) · 0★

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
