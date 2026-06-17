---
name: imazen__imageflow
source: https://github.com/imazen/imageflow/blob/7a969464777800d990e92d08cdfb4d0fbea75a9c/CLAUDE.md
repo: imazen/imageflow
kind: claude-md
stars: 4399
last_pushed: 2026-05-08T22:41:16Z
license: agpl-3.0
score: 8
domains: [systems-programming, image-processing]
tags: [simd, math-safety, visual-regression]
curated: 2026-06-15
curated_by: config-scout
---

# imazen/imageflow — claude-md

**Why it's worth keeping:** The instruction regarding `min(max)` vs `.clamp()` is a perfect example of providing 'the why' to prevent subtle, catastrophic bugs. It also clearly maps complex test workflows through a task runner (just).

**Summary:** Defines domain-specific math safety rules to prevent NaN propagation and provides structured command mappings for visual regression testing.

**Source credibility:** Highly credible; 4k+ stars and recent activity indicate a high-performance production library.

**Recency:** Current; uses modern Rust patterns and the 'just' command runner.

**Source:** [imazen/imageflow/CLAUDE.md](https://github.com/imazen/imageflow/blob/7a969464777800d990e92d08cdfb4d0fbea75a9c/CLAUDE.md) · 4399★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Imageflow Project Instructions

## SIMD & Dispatch Crates

`multiversion` is allowed in this project for autovectorization dispatch on scalar loops (e.g., `scaling.rs`). Prefer the defaults provided by `multiversed` for new code — use `multiversion` only where `multiversed` doesn't fit.

For explicit SIMD intrinsics, use `archmage` (already in use for `transpose.rs`).

## f32/f64 Clamping

**Do NOT replace `min(max(...))` patterns with `.clamp()` on floats.** `f32::clamp()` propagates NaN, while `min(max(...))` suppresses it. In image processing pipelines, NaN propagation turns a single bad pixel into a full-image corruption. The `min(max(...))` pattern is intentional NaN defense.

## Git Workflow

Always commit `cargo fmt` changes as a separate commit from code changes.

## Test Commands

All integration tests live in `imageflow_core/tests/integration/` as a single binary.

```bash
just test              # run all tests with nextest
just test-filter NAME  # run tests matching NAME
just test-update       # run tests, auto-accept checksums within tolerance
just test-replace      # reset all checksum baselines to current output
just test-list         # list all test names
just test
```

</details>
