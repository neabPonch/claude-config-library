---
name: PharmicaUK__Pharmica.AssetGen
source: https://github.com/PharmicaUK/Pharmica.AssetGen/blob/86aedf2114d7cc6762296507c441d2bae39a261b/CLAUDE.md
repo: PharmicaUK/Pharmica.AssetGen
kind: claude-md
stars: 5
last_pushed: 2026-05-18T04:36:25Z
license: mit
score: 9
domains: [dotnet, compiler-engineering, web-backend]
tags: [roslyn, source-generator, testing-frameworks, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# PharmicaUK/Pharmica.AssetGen — claude-md

**Why it's worth keeping:** Crucial detail on unique testing framework (TUnit) and the exact logic steps of the incremental generator; clear constraints regarding target frameworks (netstandard2.0 vs net9.0).

**Summary:** Provides deep technical context for a Roslyn source generator, including specific build dependencies and architectural pipelines. It explicitly defines non-standard testing frameworks to prevent LLM hallucinations.

**Source credibility:** High-quality, production-proven tool with recent activity and a well-defined purpose.

**Recency:** Very current, referencing .NET 9 technologies and modern tooling workflows.

**Source:** [PharmicaUK/Pharmica.AssetGen/CLAUDE.md](https://github.com/PharmicaUK/Pharmica.AssetGen/blob/86aedf2114d7cc6762296507c441d2bae39a261b/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Pharmica.AssetGen is a **Roslyn incremental source generator** and **diagnostic analyzer** for ASP.NET Core. It generates strongly-typed constants for wwwroot static assets (e.g., `StaticAssets.Images.LogoPng` instead of `"/images/logo.png"`), providing compile-time safety and IntelliSense.

## Build & Development Commands

```bash
dotnet tool restore          # Install CSharpier, Husky, ReportGenerator
dotnet husky install         # Install pre-commit/commit-msg git hooks
dotnet restore               # Restore NuGet packages
dotnet build                 # Build the solution
dotnet csharpier .           # Auto-format code
dotnet csharpier check .     # Check formatting (used by pre-commit hook)
```

## Testing

Uses **TUnit** (not xUnit/NUnit). Tests are async and use `Assert.That(value).IsEqualTo(expected)` style assertions.

```bash
dotnet test                                              # Run all tests
dotnet test --filter "FullyQualifiedName~AssetGenerator" # Run tests matching a pattern
dotnet test --collect:"XPlat Code Coverage"
```

</details>
