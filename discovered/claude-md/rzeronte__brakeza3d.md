---
name: rzeronte__brakeza3d
source: https://github.com/rzeronte/brakeza3d/blob/1472bea6edd1b91edb7a79e42b0a713809e33011/CLAUDE.md
repo: rzeronte/brakeza3d
kind: claude-md
stars: 79
last_pushed: 2026-06-10T17:34:45Z
license: gpl-3.0
score: 9
domains: [game-engine, graphics-programming]
tags: [cpp, opengl, architecture-patterns, build-systems]
curated: 2026-06-17
curated_by: config-scout
---

# rzeronte/brakeza3d — claude-md

**Why it's worth keeping:** Provides critical 'Key Entry Points' mappings, specific extension checklists, and hard resource limits to prevent the AI from proposing invalid or performance-breaking code.

**Summary:** A high-density technical grounding file for a custom C++ 3D engine that details build commands, architectural hierarchies, and execution flows.

**Source credibility:** Active open-source project with regular maintenance.

**Recency:** Very recent; highly optimized for modern agentic tool-use workflows.

**Source:** [rzeronte/brakeza3d/CLAUDE.md](https://github.com/rzeronte/brakeza3d/blob/1472bea6edd1b91edb7a79e42b0a713809e33011/CLAUDE.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Brakeza3D — Claude Code Instructions

@.claude/MEMORY.md

## Project
C++ 3D/2D game engine (OpenGL 3.3+, deferred rendering, ImGui editor, Lua scripting).
Version 0.26.1+, GPLv3. Build: CMake C++17, Windows/CLion primary.

## Build
```bash
# From CLion or terminal (MinGW):
cmake -B cmake-build-debug-mingw-brakezabundle -G "MinGW Makefiles" .
cmake --build cmake-build-debug-mingw-brakezabundle
```
Executable: `Brakeza3D`. Assets must be in `assets/` relative to the executable.

## Architecture at a Glance

### Frame Loop Order (critical — wrong insertion = bugs)
1. PreUpdateComponents (input, physics prep)
2. OnUpdateComponents → `Mesh3D::RunObjectShaders()` ← **object shader chain here**
3. LightPass (deferred ADS lighting)
4. PostUpdateComponents (transparent objects)
5. FlipBuffersToGlobal (layer composition)
6. PostProcessingShadersChain ← **scene shader chain here**
7. FlipGlobalToWindow → ImGui

### Key Entry Points
| Task | File |
|------|------|
| Engine loop | `src/Brakeza.cpp` |
| All components | `include/Components/Components.h` → `Components::get()` |
| Render pipeline | `src/Components/ComponentRender.cpp` |
| Post-processing | `include/Render/PostProcessingManager.h
```

</details>
