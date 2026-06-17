---
name: nanotheorygroup__kaldo
source: https://github.com/nanotheorygroup/kaldo/blob/de89b75b0d2cc346de030d1e122bf35c966d9c70/CLAUDE.md
repo: nanotheorygroup/kaldo
kind: claude-md
stars: 186
last_pushed: 2026-06-14T19:57:53Z
license: bsd-3-clause
score: 9
domains: [scientific-computing, python]
tags: [numerical-analysis, gpu-dispatch, physics]
curated: 2026-06-15
curated_by: config-scout
---

# nanotheorygroup/kaldo — claude-md

**Why it's worth keeping:** Provides crucial 'Don't' instructions (e.g., avoiding mass reformatting with new linters) and domain-specific coding standards like np.einsum usage and float comparison rules.

**Summary:** A highly technical guide for a scientific computing package that includes specific numerical best practices and architectural constraints.

**Source credibility:** Strong; comes from an active, specialized research repository for lattice dynamics.

**Recency:** Current; reflects modern Python practices and specific infrastructure requirements (TensorFlow/GPU).

**Source:** [nanotheorygroup/kaldo/CLAUDE.md](https://github.com/nanotheorygroup/kaldo/blob/de89b75b0d2cc346de030d1e122bf35c966d9c70/CLAUDE.md) · 186★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with code in this repository.

## Project overview

κALDo (kaldo) is a Python package for computing vibrational, elastic, and thermal transport properties of crystalline, disordered, and amorphous materials. It implements the Boltzmann Transport Equation (BTE) for crystals and the Quasi-Harmonic Green-Kubo (QHGK) method for disordered systems, with CPU and TensorFlow-GPU code paths. It interfaces with ab initio codes (Quantum ESPRESSO, VASP), MD packages (LAMMPS), ML potentials (NEP, MACE, MatterSim, Orb, DeepMD via ASE), and external phonon codes (ShengBTE, phono3py, hiPhive, TDEP).

## Tech stack

- Python 3.10+
- numpy, scipy, ase, sparse, opt_einsum, h5py, pandas, scikit-learn, seekpath, hiphive
- TensorFlow >= 2.13 (GPU acceleration; CPU fallback)
- pytest + pytest-cov for tests; codecov for coverage upload

## Common commands

- `pytest`: run the test suite (from repo root)
- `pytest kaldo/tests/test_crystal.py`: run a single test file
- `pytest kaldo/tests/test_crystal.py::test_name`: run one test
- `pip install -e .`: editable install for development
- CI is CircleCI (`.circleci/config.yml`)

## Project st
```

</details>
