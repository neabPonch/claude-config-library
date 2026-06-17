---
name: mjmjelde__spm
source: https://github.com/mjmjelde/spm/blob/a0f5d209f64f9e9c00fb80636d0ade2de711b2be/Claude.md
repo: mjmjelde/spm
kind: claude-md
stars: 0
last_pushed: 2026-03-20T03:51:49Z
license: mit
score: 9
domains: [cli-tools, rust, systems-programming]
tags: [phased-workflow, high-context, rust-best-practices]
curated: 2026-06-14
curated_by: config-scout
---

# mjmjelde/spm — claude-md

**Why it's worth keeping:** The 'Key Files' section teaches the AI how to distinguish between 'what' (spec) and 'how' (implementation); the explicit error handling distinction between library and CLI crates is a highly transferable professional pattern.

**Summary:** Uses a high-context system that separates specification from implementation instructions through dedicated files. It establishes a rigorous phased workflow that requires documentation updates to maintain project state.

**Source credibility:** Low star count, but the depth of engineering instruction suggests a high-quality systems project.

**Recency:** Current; reflects modern Rust best practices and structured agent workflows.

**Source:** [mjmjelde/spm/Claude.md](https://github.com/mjmjelde/spm/blob/a0f5d209f64f9e9c00fb80636d0ade2de711b2be/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md — Project Instructions for spm

## Project Overview

spm is a Rust CLI tool for building RPM and DEB packages from directory trees, with first-class support for large files (>4 GB), auto-splitting oversized packages, multi-threaded compression, and declarative `update-alternatives` integration.

**Primary use case:** Packaging large vendor software (MATLAB, CUDA, Intel compilers, EDA tools) for enterprise Linux deployment at scale.

## Key Files

- **`spec.md`** — The specification. Format constraints, YAML config schema, RPM/DEB internals, alternatives integration. This is the source of truth for *what* to build. Reference it whenever you need format details, size limits, header layouts, or config field definitions.
- **`IMPLEMENTATION.md`** — The phased build plan. Concrete Rust types, step-by-step instructions, acceptance criteria. This is *how* to build it. Work through phases in order.

## Rules

### General

- **Implement one phase at a time.** Do not skip ahead. Each phase must pass its acceptance criteria before starting the next.
- **Ask before making architectural decisions** that deviate from the spec or implementation guide. If something in the docs is wrong
```

</details>
