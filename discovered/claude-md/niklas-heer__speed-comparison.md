---
name: niklas-heer__speed-comparison
source: https://github.com/niklas-heer/speed-comparison/blob/8917f3cdf761b3b104b9e42e28d062f90a6d1ef8/CLAUDE.md
repo: niklas-heer/speed-comparison
kind: claude-md
stars: 732
last_pushed: 2026-05-19T22:18:45Z
license: mit
score: 9
domains: [benchmarking, devops, infrastructure]
tags: [build-systems, performance-testing, onboarding]
curated: 2026-06-15
curated_by: config-scout
---

# niklas-heer/speed-comparison — claude-md

**Why it's worth keeping:** Contains perfect 'how-to' patterns for project expansion and strict architectural rules that prevent AI from introducing invalid optimizations (like concurrency).

**Summary:** A highly detailed technical guide for adding new language benchmarks and navigating complex build pipelines.

**Source credibility:** High-quality, high-star benchmark repository with active maintenance and clear migration paths.

**Recency:** Highly current; uses modern tooling like Dagger, Devbox, and uv.

**Source:** [niklas-heer/speed-comparison/CLAUDE.md](https://github.com/niklas-heer/speed-comparison/blob/8917f3cdf761b3b104b9e42e28d062f90a6d1ef8/CLAUDE.md) · 732★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides context for AI assistants working on this project.

## Project Overview

A benchmark comparing 40+ programming languages using the Leibniz formula for calculating π. Results are published to GitHub Pages with historical tracking.

## Key Files

- `Earthfile` - Build definitions for all languages (Earthly build system) - **legacy**
- `dagger-poc/` - Dagger + Devbox pipeline (primary build system)
- `analyze.py` - Generates charts and CSV from benchmark results
- `publish.py` - Publishes results to `docs/history/` with timestamped folders
- `src/` - Source implementations (`leibniz.*` files)
- `src/rounds.txt` - Number of iterations (currently 1 billion)
- `scmeta/` - Crystal tool that wraps hyperfine and extracts metadata
- `docs/` - GitHub Pages site with interactive results viewer

## Build Systems

### Legacy: Earthly

Uses [Earthly](https://earthly.dev/) with Docker. Each language has a target in `Earthfile`.

### Primary: Dagger + Devbox (in `dagger-poc/`)

A Python-based pipeline using [Dagger](https://dagger.io/) and [Devbox](https://www.jetpack.io/devbox/) for better maintainability and reproducibility.

**Why Dagger + Devbox?**
- Pipeline as
```

</details>
