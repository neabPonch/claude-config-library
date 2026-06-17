---
name: superfractal__RFF-2.0-Super
source: https://github.com/superfractal/RFF-2.0-Super/blob/332b02fb1b0ad4e4e4668767184bf90897527d70/CLAUDE.md
repo: superfractal/RFF-2.0-Super
kind: claude-md
stars: 1
last_pushed: 2026-06-15T18:09:15Z
license: other
score: 8
domains: [graphics, high-performance-computing, cpp]
tags: [vulkan, math-heavy, precision-critical, rendering]
curated: 2026-06-15
curated_by: config-scout
---

# superfractal/RFF-2.0-Super — claude-md

**Why it's worth keeping:** It includes essential 'guardrail' instructions regarding precision loss and API layout alignment, plus a specific protocol for tracking AI-driven code modifications via comment tags.

**Summary:** Provides critical domain-specific technical constraints for a high-precision graphics engine involving floating-point sensitivity and Vulkan synchronization.

**Source credibility:** Low star count but the technical depth of the description suggests a highly specialized mathematical/graphics project.

**Recency:** Current; includes modern C++20 context and specific protocols for LLM modification tagging.

**Source:** [superfractal/RFF-2.0-Super/CLAUDE.md](https://github.com/superfractal/RFF-2.0-Super/blob/332b02fb1b0ad4e4e4668767184bf90897527d70/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Overview

**RFF-2.0** is a fast Mandelbrot set rendering application, built with C++20, the Vulkan API, and GMP.

- **Fast-period-guessing (FPG):** Automatically determines the longest period of the selected location.
- **Multilevel Periodic Approximation (MPA):** Skips directly to the periodic point. **This is NOT BLA** — MPA derives its skip levels from the reference orbit's *periodic structure* (see `MPAPeriod`), not from per-iteration reference magnitude. Skip lengths are variable and tied to period levels. Do not refer to it as BLA.
- **Reference Compression:** Compresses the approximation tables, heavily reducing RAM usage and skipping table-creation work.
- **Perturbation Theory:** Light and Deep perturbators compute pixel values around a high-precision reference orbit.

## Project Structure

**Core (`src/rff2/`):**

- `formula/` - Fractal computation math (`DeepMB2Perturbator`).
- `mrthy/` - Multilevel Periodic Approximation logic (`MPAPeriod`, `LightPAGenerator`).
- `vulkan/` - Graphics/Compute pipelines (`GPC*` graphics, `CPC*` compute): palettes, blurs, blooms, fractals.
- `ui/` - Win32 UI, window callbacks, and `RenderScene`.
- `io/` - Maps, videos, and locati
```

</details>
