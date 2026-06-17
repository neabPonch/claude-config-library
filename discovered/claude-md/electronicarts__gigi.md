---
name: electronicarts__gigi
source: https://github.com/electronicarts/gigi/blob/401386cfd7c6e39e549d939e44d99bd5b49cd14d/CLAUDE.md
repo: electronicarts/gigi
kind: claude-md
stars: 1165
last_pushed: 2026-05-21T17:43:28Z
license: other
score: 9
domains: [graphics-engine, compiler-design, cli-tools]
tags: [rendering, code-generation, schema-driven, graphics-api]
curated: 2026-06-15
curated_by: config-scout
---

# electronicarts/gigi — claude-md

**Why it's worth keeping:** It includes high-value architecture patterns (schema-driven design) and specific verification workflows involving both runtime scripts and diff-checking generated code.

**Summary:** Provides a deep mental model of a complex multi-component rendering framework, covering the full pipeline from JSON schemas to backend code generation.

**Source credibility:** High; authored by Electronic Arts with significant community traction (1k+ stars).

**Recency:** Highly current, including modern MCP implementation details.

**Source:** [electronicarts/gigi/CLAUDE.md](https://github.com/electronicarts/gigi/blob/401386cfd7c6e39e549d939e44d99bd5b49cd14d/CLAUDE.md) · 1165★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Gigi is a rapid graphics prototyping and code generation suite for real-time rendering techniques. It consists of four main components:

1. **GigiEdit** - Editor for authoring rendering techniques as node graphs (`.gg` files)
2. **GigiViewerDX12** - Viewer for running, debugging, and profiling techniques with Python scripting
3. **GigiCompiler** - Command-line compiler that generates platform-specific code from `.gg` files
4. **GigiBrowser** - Browser for viewing and submitting techniques to the library

The core concept: users describe rendering techniques as graphs of nodes in the editor. Gigi compiles these to human-readable code for various backends (DX12, UE5, WebGPU, Frostbite, etc.).

## Building

Build the entire project:
```bash
# Open and build the solution in Visual Studio
# Both Debug and Release configurations target x64
```

The solution file `gigi.sln` includes all components. After building, executables appear in the root directory.

## Testing

### Viewer Unit Tests
Run from within GigiViewerDX12:
```
File -> Run Python Script ->
```

</details>
