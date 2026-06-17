---
name: atopile__atopile
source: https://github.com/atopile/atopile/blob/619eda7f777558a3e500dbad9cc2941712881495/CLAUDE.md
repo: atopile/atopile
kind: claude-md
stars: 3402
last_pushed: 2026-06-13T02:58:22Z
license: mit
score: 9
domains: [eda, systems-programming, monorepo]
tags: [modular-skills, monorepo-structure, entry-point-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# atopile/atopile — claude-md

**Why it's worth keeping:** Uses a sophisticated 'Skills' architecture that decomposes domain expertise into modular sub-files rather than one monolithic file; includes a clear mapping of modules to their execution entry points.

**Summary:** Provides a highly structured map of a complex monorepo, linking modules to specific entry points and languages.

**Source credibility:** Highly credible source with 3.4k stars and active maintenance.

**Recency:** Very recent, specifically optimized for agentic workflows using specialized context directories.

**Source:** [atopile/atopile/CLAUDE.md](https://github.com/atopile/atopile/blob/619eda7f777558a3e500dbad9cc2941712881495/CLAUDE.md) · 3402★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Overview

You are inside the atopile monorepo.
atopile is an open-source EDA tool.
ato is a domain-specific language that is created to define electronics in code.
Everything is modeled in the graph.
There multiple layers and modules:
zig, graph, faebryk, fabll, domain-layer, build-server, frontend

## Modules & Entry Points

| Module           | Location                                  | Entry Point                                                                      |
| ---------------- | ----------------------------------------- | -------------------------------------------------------------------------------- |
| **zig**          | `src/faebryk/core/zig/`                   | `build.zig` → compiles to `pyzig` extension                                      |
| **graph**        | `src/faebryk/core/zig/src/graph/`         | `lib.zig` (bindings in `src/faebryk/core/zig/src/python/graph/manual/graph.pyi`) |
| **faebryk**      | `src/faebryk/core/zig/src/faebryk`        | `lib.zig` (bindings in `src/faebryk/core/zig/src/python/faebryk/manual`)         |
| **fabll**        | `src/faebryk/core/node.py`                |
```

</details>
