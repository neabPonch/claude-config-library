---
name: EiffL__LatentInverseProblems
source: https://github.com/EiffL/LatentInverseProblems/blob/a86fbc6d05ea0240c3abfa0d4342a106fa9047ae/CLAUDE.md
repo: EiffL/LatentInverseProblems
kind: claude-md
stars: 0
last_pushed: 2026-03-14T00:26:14Z
license: mit
score: 8
domains: [scientific-computing, machine-learning, research]
tags: [jax, diffusion, mathematical-modeling]
curated: 2026-06-16
curated_by: config-scout
---

# EiffL/LatentInverseProblems — claude-md

**Why it's worth keeping:** The 'Key Dependencies and Patterns' section includes specific technical caveats to prevent library-version errors, while the module descriptions provide mathematical signatures crucial for LLM-driven development.

**Summary:** Defines high-level research objectives and maps out a complex scientific codebase using JAX. It provides clear paths for both running benchmarks and rapid prototyping.

**Source credibility:** Low star count indicates a niche personal research project, but the content is highly structured and expert-level.

**Recency:** Current; addresses modern dependency nuances like diffrax 0.7+ requirements.

**Source:** [EiffL/LatentInverseProblems/CLAUDE.md](https://github.com/EiffL/LatentInverseProblems/blob/a86fbc6d05ea0240c3abfa0d4342a106fa9047ae/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Goal

Identify a reliable and correct strategy for **diffusion posterior sampling in latent space** that produces **calibrated posteriors** suitable for scientific applications (cosmology, medical imaging, geophysics). We benchmark methods on **MNISTVAE** -- a pretrained VAE decoder on MNIST where the exact posterior is available via grid evaluation.

**Central open problem:** No existing diffusion-based method provides calibrated posteriors with latent diffusion models. The decoder Jacobian distortion, representation error, and decoder nonlinearity remain unsolved.

**For research loop instructions, see `program.md`.** Current best results are in `results/scoreboard.md`.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e .                   # installs lip package (jax)
pip install -r requirements.txt    # additional deps: diffrax, numpyro, optax
```

Python 3.14 venv is already present at `.venv/`.

## Running Benchmarks

```bash
python scripts/run_mnist_vae.py    # MNISTVAE benchmark (all solvers)
python experiment.py
```

</details>
