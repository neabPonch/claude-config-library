---
name: fernforestgames__luau-gdextension
source: https://github.com/fernforestgames/luau-gdextension/blob/bc1b88da7121a6b049094a5eebc7e5b359bc8ac3/CLAUDE.md
repo: fernforestgames/luau-gdextension
kind: claude-md
stars: 22
last_pushed: 2026-05-28T18:21:04Z
license: mit
score: 9
domains: [game-engine, systems-programming, c++]
tags: [godot, gdextension, luau, cmake]
curated: 2026-06-15
curated_by: config-scout
---

# fernforestgames/luau-gdextension — claude-md

**Why it's worth keeping:** The instruction to use `doc_classes/*.xml` as a single source of truth and providing specific pattern warnings (e.g., `to_string_inplace`) are elite techniques for preventing LLM hallucinations. It also includes ready-to-use platform-specific build commands.

**Summary:** Highly specific technical manual that establishes XML documentation as the authoritative source of truth for API signatures. It provides exact build/test commands and high-value 'Do/Don't' patterns to prevent common C++/Godot errors.

**Source credibility:** Niche project with active maintenance (last push 1 month ago).

**Recency:** Highly current, utilizing Godot 4.5+ and modern CMake presets.

**Source:** [fernforestgames/luau-gdextension/CLAUDE.md](https://github.com/fernforestgames/luau-gdextension/blob/bc1b88da7121a6b049094a5eebc7e5b359bc8ac3/CLAUDE.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Documentation

**IMPORTANT: The authoritative API reference is in `doc_classes/*.xml`.** These
XML files are the single source of truth for all exposed classes, methods,
constants, and their parameters. They are compiled into the GDExtension and
appear in Godot's built-in help system.

When working with this codebase:
1. **Always consult `doc_classes/` for accurate API signatures** - method names,
   parameter types, default values, and return types
2. Keep CLAUDE.md examples up-to-date with the doc_classes/ API
3. Update doc_classes/ XML files when adding or modifying public APIs
4. Use `godot --doctool` to regenerate documentation after API changes

**Common API patterns:**
- To get a string from the stack: Use `to_string_inplace(index)`, NOT `to_string(index)`
- To get any value as a Variant: Use `to_variant(index)`
- To set a global: Use `set_global(key)` after pushing the value (NOT `set_global(key, value)`)

## Project Overview

A Godot 4.5+ GDExtension that integrates the Luau scripting language (Lua
derivative) into Godot Engine.

**Core Classes:**

- `Lua
```

</details>
