---
name: libAtoms__QUIP
source: https://github.com/libAtoms/QUIP/blob/1e2f84ba94bc715a5d7b0b0c7c2ba1b2d402e730/CLAUDE.md
repo: libAtoms/QUIP
kind: claude-md
stars: 396
last_pushed: 2026-05-12T08:49:18Z
license: unknown
score: 9
domains: [scientific-computing, fortran, physics-simulations]
tags: [build-system, architecture, development-patterns, molecular-dynamics]
curated: 2026-06-15
curated_by: config-scout
---

# libAtoms/QUIP — claude-md

**Why it's worth keeping:** Includes 'Common Development Patterns' that guide the agent through specific extension tasks; provides deep architectural context including module hierarchies and file format specifications; highlights domain-specific nuances like pre-processing differences.

**Summary:** Provides comprehensive instructions for building, testing, and extending a complex Fortran-based molecular dynamics framework with Python bindings.

**Source credibility:** High-quality scientific software repository (libAtoms/QUIP) with significant community interest.

**Recency:** Modern; utilizes Meson build system and current Python integration patterns.

**Source:** [libAtoms/QUIP/CLAUDE.md](https://github.com/libAtoms/QUIP/blob/1e2f84ba94bc715a5d7b0b0c7c2ba1b2d402e730/CLAUDE.md) · 396★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

QUIP (QUantum mechanics and Interatomic Potentials) is a collection of Fortran software tools for molecular dynamics simulations. It implements various interatomic potentials, tight binding quantum mechanics, and can interface with external packages like LAMMPS, CP2K, and ASE. The codebase includes:

- **Core library (libAtoms)**: Fundamental atomistic data structures and algorithms
- **Interatomic Potentials**: Various potential models (EAM, Tersoff, Stillinger-Weber, Lennard-Jones, etc.)
- **GAP (Gaussian Approximation Potentials)**: Machine learning interatomic potentials (separate license - Academic Software License)
- **Python interface (quippy)**: Python bindings via f90wrap for integration with ASE
- **Tight-binding modules**: DFTB, NRL-TB, and other TB implementations
- **Analysis programs**: 50+ Fortran utilities in `src/Programs/`

## Build System

QUIP uses the [Meson build system](https://mesonbuild.com/) (version 1.1+) with the Ninja build tool.

### Initial Setup

1. Ensure you have the required tools:
```bash
pip install meson ninja
```

2
```

</details>
