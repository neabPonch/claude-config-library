---
name: TuringLang__Turing.jl
source: https://github.com/TuringLang/Turing.jl/blob/f6f9d13985b9f1e7fff50ee8e5741d4b9eac0b8d/CLAUDE.md
repo: TuringLang/Turing.jl
kind: claude-md
stars: 2243
last_pushed: 2026-06-14T05:04:02Z
license: mit
score: 9
domains: [scientific-computing, data-science, mathematics]
tags: [julia, probabilistic-programming, architecture-guidelines, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# TuringLang/Turing.jl — claude-md

**Why it's worth keeping:** The 'Review Guidelines' section is elite; it explains the technical rationale behind specific API choices (e.g., why to use OnlyAccsVarInfo over VarInfo), allowing Claude to perform high-quality code reviews rather than just writing code.

**Summary:** Provides architectural hierarchy, build/test commands, and strict coding standards for a complex scientific computing library.

**Source credibility:** High: Turing.jl is a foundational, highly-starred library in the Julia probabilistic programming ecosystem.

**Recency:** Current; reflects recent architectural shifts and specific tool versions (JuliaFormatter v1).

**Source:** [TuringLang/Turing.jl/CLAUDE.md](https://github.com/TuringLang/Turing.jl/blob/f6f9d13985b9f1e7fff50ee8e5741d4b9eac0b8d/CLAUDE.md) · 2243★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Turing.jl is the user-facing entry point for the [TuringLang](https://github.com/TuringLang) probabilistic programming ecosystem. It is largely a translation layer between DynamicPPL models — which work with named, structured parameters — and inference algorithms that expect flat, vectorised samples (e.g. HMC/NUTS operate on `AbstractVector{<:Real}`). DynamicPPL's `LogDensityFunction` handles most of this translation; Turing provides the sampler wrappers that set it up and manage state across iterations.

Model definition lives in [DynamicPPL.jl](https://github.com/TuringLang/DynamicPPL.jl), parameter transformations in [Bijectors.jl](https://github.com/TuringLang/Bijectors.jl), and sampling interfaces in [AbstractMCMC.jl](https://github.com/TuringLang/AbstractMCMC.jl). Turing re-exports their APIs and provides concrete sampler implementations that wire everything together.

## Building and Testing

Code formatting uses [JuliaFormatter.jl](https://github.com/domluna/JuliaFormatter.jl) v1 (not v2) with the **Blue style** (configured in `.JuliaForm
```

</details>
