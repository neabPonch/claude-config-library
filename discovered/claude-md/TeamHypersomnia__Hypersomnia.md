---
name: TeamHypersomnia__Hypersomnia
source: https://github.com/TeamHypersomnia/Hypersomnia/blob/6e8d8a326efb9585028f83dd7a7c8a177c089129/CLAUDE.md
repo: TeamHypersomnia/Hypersomnia
kind: claude-md
stars: 1567
last_pushed: 2026-06-07T09:44:00Z
license: agpl-3.0
score: 9
domains: [cpp, game-dev, systems-programming]
tags: [coding-standards, mcp, build-tools, cpp]
curated: 2026-06-15
curated_by: config-scout
---

# TeamHypersomnia/Hypersomnia — claude-md

**Why it's worth keeping:** The use of explicit code snippets for complex patterns like 'const via lambda' is excellent; it also shows how to bridge the gap between LLM capabilities and unique build workflows through MCP instructions.

**Summary:** Provides hyper-specific C++ coding standards (spacing, indentation, pattern usage) and detailed definitions for a custom MCP build toolset.

**Source credibility:** High-quality repository with 1500+ stars and very recent updates.

**Recency:** Highly current, as it includes specific integration for MCP (Model Context Protocol) tools.

**Source:** [TeamHypersomnia/Hypersomnia/CLAUDE.md](https://github.com/TeamHypersomnia/Hypersomnia/blob/6e8d8a326efb9585028f83dd7a7c8a177c089129/CLAUDE.md) · 1567★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
**No yapping.** To the point language. Speak like a caveman, but dont remove tenses: keep "used", "uses". Keep "a", "an", "the".

# Build tools (MCP)

A `build` MCP server is available with four tools:
- `build_file <path>` — compile a single `.cpp` (path relative to repo root) for fast error-checking after edits
- `build` — full ninja build
- `build_cmake` — regenerate CMake build files when `CMakeLists.txt` changes
- `cmake_debug_fast` — generate the fast-building Debug configuration: runs `BUILD_FOLDER_SUFFIX=fast cmake/build.sh Debug x64 -DGENERATE_DEBUG_INFORMATION=0`, creates `build/Debug-x64-clang-fast/` and symlinks `build/current` to it

`build`, `build_cmake`, and `build_file` will first run `cmake_debug_fast` if the `build/` folder does not yet exist.

Prefer `build_file` to verify edits to a specific file before running a full `build`.

# General programming rules

- **Do not change formatting style like tabs or other spacing conventions in the files you are editing.**

- Don't automatically commit unless I ask to.

- Include order
	- Standard libraries first
	- Then in the order of basic to specific: augs -> game -> view -> application, e.g.:
		```cpp
		#include <vecto
```

</details>
