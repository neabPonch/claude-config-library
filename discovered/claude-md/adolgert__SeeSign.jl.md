---
name: adolgert__SeeSign.jl
source: https://github.com/adolgert/SeeSign.jl/blob/000489288a9d58e935001a3eb572fca1397c42d8/CLAUDE.md
repo: adolgert/SeeSign.jl
kind: claude-md
stars: 0
last_pushed: 2025-11-24T23:49:25Z
license: mit
score: 7
domains: [scientific-computing, simulation]
tags: [julia, mathematical-modeling, discrete-event-simulation]
curated: 2026-06-16
curated_by: config-scout
---

# adolgert/SeeSign.jl — claude-md

**Why it's worth keeping:** It uses comparative programming context to prevent language-specific mistakes and defines a strict architectural philosophy regarding defensive coding and documentation.

**Summary:** Establishes mathematical design principles for a simulation framework and provides critical technical distinctions between Julia and Python.

**Source credibility:** Low social proof (0 stars), likely a specialized research or single-author project.

**Recency:** Current; the language differences provided are fundamental to Julia's architecture.

**Source:** [adolgert/SeeSign.jl/CLAUDE.md](https://github.com/adolgert/SeeSign.jl/blob/000489288a9d58e935001a3eb572fca1397c42d8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Project Context

This project is a framework for Statistics. The closer the code is to the statistical process for Generalized Semi-Markov Processes, the better the code will be. Use the right data structures and algorithms for the mathematical function.

## Julia language

You are new to Julia. Here are differences between Julia and Python.

 * If there is a package you want to use, check that this package is in Project.toml. If it is not in Project.toml, you can add it with `julia -e 'using Pkg; Pkg.add("PackageName")'`.

 * A struct defined with "struct" is immutable by default. If you want to define a mutable struct, you need to use "mutable struct".

 * You can't define a struct within a function, even though Python can do this.

 * The `yield` keyword is about tasks in Julia, not about coroutines.

## Code Hygiene

 * Defensive coding is a mistake unless it is checking a user's inputs. We define preconditions, postconditions, and invariants, and we rely on them.

 * For this repository, please limit comments to "WHY code is written this way". If the code is self-explanatory, you can leave it uncommented.

 * Two spaces between functions for better legibility.

## Tools

 *
```

</details>
