---
name: jakildev__IrredenEngine__claude
source: https://github.com/jakildev/IrredenEngine/blob/088533a414794e6f13597c1b0724ed7edeba6973/engine/script/CLAUDE.md
repo: jakildev/IrredenEngine
kind: claude-md
stars: 8
last_pushed: 2026-06-16T03:18:51Z
license: mit
score: 9
domains: [game-engine, systems-programming]
tags: [lua-jit, ecs, cpp, bindings]
curated: 2026-06-16
curated_by: config-scout
---

# jakildev/IrredenEngine — claude-md

**Why it's worth keeping:** It defines strict architectural requirements for extending the system (the trait-based pattern) and provides specific 'gotchas' regarding LuaJIT/Sol2 that prevent common logic errors.

**Summary:** Provides deep technical context for a C++/LuaJIT bridge in a custom ECS engine. It covers binding patterns, runtime limitations, and component registration rules.

**Source credibility:** High-quality documentation from an active, structured game engine project.

**Recency:** Extremely current; repository was updated months ago/recently.

**Source:** [jakildev/IrredenEngine/engine/script/CLAUDE.md](https://github.com/jakildev/IrredenEngine/blob/088533a414794e6f13597c1b0724ed7edeba6973/engine/script/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# engine/script/ — LuaJIT 2.1 via sol2

Thin wrapper around sol2 that exposes ECS components, math, and input to
Lua. Creations register *which* components get bound via a per-creation
`lua_component_pack.hpp` file.

## Lua runtime: LuaJIT 2.1

The engine's Lua VM is **LuaJIT 2.1** (Lua 5.1 base + LuaJIT extensions).
The runtime is fetched at configure time and built from upstream source
via `engine/script/third_party/luajit/CMakeLists.txt`.

What's available beyond Lua 5.1:

- `bit` module — bitwise ops over 32-bit integers (LuaJIT-native, faster
  than Lua 5.4's `>>`/`<<`/`&`/`|` operators when JIT-compiled).
- `ffi` module — C FFI from Lua. Available to creations; engine bindings
  stay sol2-based.
- Trace JIT compiler — heats up stable inner loops into compiled native
  code. Per-archetype Lua system ticks are exactly the shape it
  compiles well; expect 2–10× C++ on warmed-up loops vs. ≥10 000× under
  the prior Lua 5.4 + sol2 path.

What's NOT available (Lua 5.2/5.3/5.4 features, do not use):

- `goto` / labels — LuaJIT runs in 5.1-compat mode by default.
- Integer subtype — all numbers are doubles; whole-number literals
  written `0`, `0.0`, or `1.0` round-trip identically t
```

</details>
