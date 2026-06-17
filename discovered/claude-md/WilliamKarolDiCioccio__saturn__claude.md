---
name: WilliamKarolDiCioccio__saturn__claude
source: https://github.com/WilliamKarolDiCioccio/saturn/blob/205e3e1ba873700cdc294b2ec69ab3561930e32e/saturn/graphics/CLAUDE.md
repo: WilliamKarolDiCioccio/saturn
kind: claude-md
stars: 3
last_pushed: 2026-05-25T23:29:57Z
license: agpl-3.0
score: 9
domains: [game-engine, graphics-api, cpp]
tags: [architectural-constraints, invariants, ownership-models]
curated: 2026-06-15
curated_by: config-scout
---

# WilliamKarolDiCioccio/saturn — claude-md

**Why it's worth keeping:** It utilizes 'Owns vs Does NOT Own' sections to prevent scope creep and provides specific line-number references for key types to improve LLM navigation.

**Summary:** This file defines the strict architectural boundaries, ownership rules, and lifecycle invariants for a graphics engine module.

**Source credibility:** High-quality engineering documentation from a specialized C++ game engine project.

**Recency:** Extremely relevant as it provides the structural context required for complex system maintenance in Claude Code.

**Source:** [WilliamKarolDiCioccio/saturn/saturn/graphics/CLAUDE.md](https://github.com/WilliamKarolDiCioccio/saturn/blob/205e3e1ba873700cdc294b2ec69ab3561930e32e/saturn/graphics/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Package: saturn/graphics

**Location:** `saturn/include/saturn/graphics/`, `saturn/src/graphics/`
**Type:** Part of saturn shared/static library
**Dependencies:** pieces (Result), window/ (Window), core/ (System), Vulkan SDK (volk, VMA), WebGPU (Dawn/Emscripten)

---

## Purpose & Responsibility

### Owns

- Rendering abstraction layer (RenderSystem, RenderContext)
- Backend implementations (Vulkan, WebGPU)
- Frame lifecycle (beginFrame → updateResources → drawScene → endFrame)
- Surface creation and swapchain management
- GPU memory allocation (VMA for Vulkan)
- Command buffer recording and submission
- Render pass management
- Pipeline and shader compilation
- Per-window render contexts (multi-window support)

### Does NOT Own

- Window creation (window/ package)
- Input handling (input/ package)
- Scene graph or entity management (scene/ and ecs/ packages)
- Asset loading (textures, models, shaders from disk)
- High-level rendering API (materials, meshes, lights - user code)

---

## Key Abstractions & Invariants

### Core Types

- **`RenderSystem`** (`render_system.hpp:26`) — EngineSystem base, owns contexts, factory pattern, singleton
- **`RendererAPIType`** (`render_system.
```

</details>
