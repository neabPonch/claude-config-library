---
name: Cysharp__ZLinq
source: https://github.com/Cysharp/ZLinq/blob/357a6382acffb612764bdfe6f0fe1ba9971878d5/CLAUDE.md
repo: Cysharp/ZLinq
kind: claude-md
stars: 5159
last_pushed: 2026-06-12T02:33:06Z
license: mit
score: 9
domains: [dot-net, high-performance-computing, game-dev]
tags: [dotnet, linq, performance, unity]
curated: 2026-06-16
curated_by: config-scout
---

# Cysharp/ZLinq — claude-md

**Why it's worth keeping:** It lists critical 'cannot do' rules (like no yield return or IEnumerable conversion) that prevent an LLM from breaking the core performance architecture. It also includes highly specific style constraints like field naming conventions to ensure consistency.

**Summary:** Provides deep architectural context for a zero-allocation LINQ library, including specific technical constraints and optimization patterns.

**Source credibility:** Very high; Cysharp is a premier source for high-performance .NET and Unity optimizations.

**Recency:** Current; references .NET 9, VS Preview, and modern testing frameworks.

**Source:** [Cysharp/ZLinq/CLAUDE.md](https://github.com/Cysharp/ZLinq/blob/357a6382acffb612764bdfe6f0fe1ba9971878d5/CLAUDE.md) · 5159★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ZLinq is a zero-allocation LINQ library for .NET that provides high-performance alternatives to System.Linq through struct-based value types. The library offers LINQ to Span, LINQ to SIMD, and LINQ to Tree functionality across all .NET platforms including Unity and Godot.

## Key Architecture

### Core Design
- **ValueEnumerable<TEnumerator, T>**: Main struct that wraps enumerators to enable method chaining without allocations
- **IValueEnumerator<T>**: Interface defining `TryGetNext(out T current)` pattern instead of MoveNext/Current
- **ref struct support**: In .NET 9+, ValueEnumerable is a ref struct enabling Span<T> integration
- **Optimization methods**: `TryGetNonEnumeratedCount`, `TryGetSpan`, `TryCopyTo` for performance optimizations

### Project Structure
- `src/ZLinq/`: Core library with all LINQ operators in `Linq/` folder and SIMD implementations in `Simd/`
- `src/ZLinq.DropInGenerator/`: Source generator for automatic ZLinq method replacement
- `src/ZLinq.FileSystem/`, `ZLinq.Json/`, `ZLinq.Godot/`: Tree traversal extensions
- `src/Z
```

</details>
