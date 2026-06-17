---
name: DifferentiableUniverseInitiative__jax_cosmo
source: https://github.com/DifferentiableUniverseInitiative/jax_cosmo/blob/c4f249f3712f2c4fe4b526274baad41a48e187ac/CLAUDE.md
repo: DifferentiableUniverseInitiative/jax_cosmo
kind: claude-md
stars: 240
last_pushed: 2025-06-27T16:56:12Z
license: mit
score: 8
domains: [scientific-computing, physics]
tags: [jax, cosmology, differentiation, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# DifferentiableUniverseInitiative/jax_cosmo — claude-md

**Why it's worth keeping:** The 'Container Class Pattern' example and explicit rules against Python control flow prevent the AI from writing code that breaks XLA/autograd.

**Summary:** Provides deep architectural context for JAX-specific programming patterns to ensure end-to-end differentiability.

**Source credibility:** High; 240 stars indicates a respected, specialized scientific tool in the cosmology community.

**Recency:** Current; aligns perfectly with modern JAX-centric development workflows.

**Source:** [DifferentiableUniverseInitiative/jax_cosmo/CLAUDE.md](https://github.com/DifferentiableUniverseInitiative/jax_cosmo/blob/c4f249f3712f2c4fe4b526274baad41a48e187ac/CLAUDE.md) · 240★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

jax-cosmo is a differentiable cosmology library built on JAX, providing end-to-end automatic differentiation for cosmological computations. It enables efficient inference (HMC, VI) and survey optimization tasks by computing observables like angular power spectra and correlation functions for various tracers (lensing, clustering, CMB lensing).

## Development Commands

### Testing
```bash
pytest                    # Run all tests
pytest tests/test_*.py    # Run specific test file
```

### Code Formatting
```bash
black .                   # Format code with Black
```

### Installation
```bash
pip install -e .          # Install in development mode
pip install -e .[test]    # Install with test dependencies
```

### Documentation
```bash
cd docs && make html      # Build documentation with Sphinx
```

## Architecture

### Core Design Principles
- **JAX-first**: All functions must be JAX-compatible for automatic differentiation
- **Avoid Python loops**: Use `jax.vmap` or `jax.lax` for XLA-compatible operations
- **Functions over methods**: Enable `jax.grad(fu
```

</details>
