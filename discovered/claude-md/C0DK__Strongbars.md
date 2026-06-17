---
name: C0DK__Strongbars
source: https://github.com/C0DK/Strongbars/blob/c837b307edacf809d37c6be2dbc8654990240211/CLAUDE.md
repo: C0DK/Strongbars
kind: claude-md
stars: 1
last_pushed: 2026-05-19T14:42:58Z
license: unknown
score: 9
domains: [dotnet, dev-tools]
tags: [csharp, source-generator, ast, templating]
curated: 2026-06-17
curated_by: config-scout
---

# C0DK/Strongbars — claude-md

**Why it's worth keeping:** It provides essential DSL syntax rules and architectural deep-dives (like the AST structure) that allow an LLM to modify the generator's core logic without manual exploration. It also explicitly documents known technical limitations to prevent hallucinations.

**Summary:** A highly detailed technical guide for a .NET source generator that details syntax, AST architecture, and build-time logic.

**Source credibility:** Low star count, but high-quality documentation indicates a sophisticated developer/author.

**Recency:** Extremely current; pushed 1 month ago and uses modern .NET patterns.

**Source:** [C0DK/Strongbars/CLAUDE.md](https://github.com/C0DK/Strongbars/blob/c837b307edacf809d37c6be2dbc8654990240211/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Strongbars Codebase Guide

## Project Overview

**Strongbars** is a compile-time, type-safe .NET source generator that transforms text templates (HTML, JSON, SQL, etc.) containing `{{variable}}` placeholder syntax into strongly-typed C# classes. The key design goal is zero runtime overhead and build-time validation of template parameters.

Published on NuGet as two packages:
- `Strongbars` — main package users reference
- `Strongbars.Abstractions` — base types that generated classes inherit from

---

## Repository Structure

```
Strongbars/
├── Strongbars/                     # NuGet package shell (no real C# code)
│   ├── Strongbars.csproj           # Version, NuGet metadata, package bundling
│   └── build/
│       └── Strongbars.props        # MSBuild props injected into consumer projects
├── Strongbars.Abstractions/        # Base types for generated classes
│   ├── Template.cs                 # Base class: Template : TemplateArgument
│   ├── Variable.cs                 # Variable metadata (name, type, optional, array)
│   └── VariableType.cs             # Enum: String, IFormattable, TemplateArgument, Bool
├── Strongbars.Generator/           # The actual source gen
```

</details>
