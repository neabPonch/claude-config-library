---
name: drumtorben__polars-ts
source: https://github.com/drumtorben/polars-ts/blob/a2229d6a50c8d2fff1e97453e02f12126e68e7e7/CLAUDE.md
repo: drumtorben/polars-ts
kind: claude-md
stars: 41
last_pushed: 2026-06-08T12:41:06Z
license: unknown
score: 9
domains: [data-science, backend-systems]
tags: [knowledge-graph, tech-debt, rust-ffi, agent-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# drumtorben/polars-ts — claude-md

**Why it's worth keeping:** The 'graphify' loop is a sophisticated way to keep agentic mental models synced with code changes, while the 'Tech Debt Hotspots' section provides high-signal instructions for refactoring instead of vague descriptions.

**Summary:** Integrates a local knowledge graph system (graphify) to maintain structural context and provides high-density maps of technical debt. It uses specific dispatch rules to prevent import errors in a complex hybrid Python/Rust environment.

**Source credibility:** Highly credible; recently active (0 months ago) and contains complex, domain-specific technical architecture.

**Recency:** Very current; utilizes modern Python 3.12 standards and advanced agentic workflows.

**Source:** [drumtorben/polars-ts/CLAUDE.md](https://github.com/drumtorben/polars-ts/blob/a2229d6a50c8d2fff1e97453e02f12126e68e7e7/CLAUDE.md) · 41★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## graphify

This project has a graphify knowledge graph at graphify-out/.

Rules:
- Before answering architecture or codebase questions, read graphify-out/GRAPH_REPORT.md for god nodes and community structure
- If graphify-out/wiki/index.md exists, navigate it instead of reading raw files
- After modifying code files in this session, run `python3 -c "from graphify.watch import _rebuild_code; from pathlib import Path; _rebuild_code(Path('.'))"` to keep the graph current

## Project Architecture

- **Hybrid Python/Rust codebase**: Python package at `polars_ts/`, Rust FFI via `polars_ts_rs` (built with maturin) at `src/`
- **Lazy imports**: All submodule `__init__.py` files should use `polars_ts._lazy.make_getattr` pattern
- **Distance dispatch**: `_distance_dispatch.py` is the canonical location for Rust distance function imports; other modules should import from there, not directly from `polars_ts_rs`
- **Shared helpers**: `pipeline.py` owns `_build_feature_df`, `_apply_transform`, `_build_step_features`; `global_model.py` imports from there
- **Time utils**: `_infer_freq` and `_make_future_dates` live in `models/baselines.py` (canonical) — `models/arima.py` has its own copy (tech
```

</details>
