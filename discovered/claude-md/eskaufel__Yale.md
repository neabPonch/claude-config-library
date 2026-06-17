---
name: eskaufel__Yale
source: https://github.com/eskaufel/Yale/blob/0f015665b316a6d688b0d0f947a4b8b1b5de9642/CLAUDE.md
repo: eskaufel/Yale
kind: claude-md
stars: 4
last_pushed: 2026-06-08T04:04:30Z
license: lgpl-3.0
score: 8
domains: [.net, compiler-design]
tags: [dotnet, compilers, library]
curated: 2026-06-15
curated_by: config-scout
---

# eskaufel/Yale — claude-md

**Why it's worth keeping:** The 'Architecture Notes' explain the high-level logic flow (Parser to CIL), while specific 'Code Style' rules prevent stylistic drift during AI-led refactoring.

**Summary:** A detailed technical blueprint for a .NET library, covering directory structure, build/test procedures, and core architectural flows.

**Source credibility:** Well-structured, specialized .NET tool with clear maintenance documentation.

**Recency:** Current; reflects modern .NET development and tooling standards.

**Source:** [eskaufel/Yale/CLAUDE.md](https://github.com/eskaufel/Yale/blob/0f015665b316a6d688b0d0f947a4b8b1b5de9642/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Yale – Claude Code Context

## Project Overview

Yale is a .NET 6.0 expression parser and evaluator library. It compiles string expressions (e.g., `sqrt(a^2 + b^2)`, `name() = "Maria"`) to Common Intermediate Language (CIL) for fast runtime evaluation. It is a modernization of the [Flee](https://github.com/mparlak/Flee) library. Licensed under LGPL-3.0.

## Repository Structure

```
src/Yale/
  Expression/         # Expression compilation pipeline
    Elements/         # Operator and literal AST nodes
    Elements/Base/    # Base classes for expression elements
    Elements/Literals/
    Elements/LogicalBitwise/
    Elements/MemberElements/
  Core/Interfaces/    # Public-facing interfaces
  Engine/             # Compilation entry points (ComputeInstance, options)
    Interface/
    Internal/
  Parser/             # Tokenizer / grammar (RE/, Internal/)
  Resources/          # Localized error message .resx files
test/Yale.Tests/      # MSTest unit tests
  Core/, Engine/, ExpressionTests/, Parser/, Theory/, Helper/
benchmark/Yale.Benchmarks/  # BenchmarkDotNet suite (Parse/, Engine/)
```

## Build & Test Commands

```bash
# Restore dependencies
dotnet restore

# Build (debug)
dotnet
```

</details>
