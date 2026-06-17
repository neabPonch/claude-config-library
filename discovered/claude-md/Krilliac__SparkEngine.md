---
name: Krilliac__SparkEngine
source: https://github.com/Krilliac/SparkEngine/blob/0d0dae01666f6108e7f2da6cd42871e8d093e923/CLAUDE.md
repo: Krilliac/SparkEngine
kind: claude-md
stars: 19
last_pushed: 2026-06-15T03:54:47Z
license: other
score: 9
domains: [game-engine, systems-programming]
tags: [anti-bloat, modern-cpp, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# Krilliac/SparkEngine — claude-md

**Why it's worth keeping:** The 'Anti-Bloat Guidelines' with numeric thresholds and the 'Bloat Check' shell command are brilliant, transferable patterns for maintaining large codebases. The detailed directory map also provides immediate spatial awareness for navigating complex systems.

**Summary:** Establishes a rigorous 'session start' ritual that includes git synchronization and proactive code bloat auditing. It provides highly specific architectural constraints to prevent AI-driven over-engineering.

**Source credibility:** Active, high-performance C++23 game engine project.

**Recency:** Highly current; utilizes modern C++ standards and specific session-start rituals designed for AI agents.

**Source:** [Krilliac/SparkEngine/CLAUDE.md](https://github.com/Krilliac/SparkEngine/blob/0d0dae01666f6108e7f2da6cd42871e8d093e923/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SparkEngine — Claude Code Context

## What is this?

SparkEngine is a C++23 open-source 3D game engine (with C++26 forward-compatibility macros). Originally focused on first-person shooters, it is evolving into a general-purpose engine supporting FPS, RPG, MMO, open-world, and other genres.
- **Rendering**: Full RHI abstraction — D3D11 (primary), D3D12/Vulkan/Metal/OpenGL (experimental backends)
- **Physics**: Jolt Physics
- **Audio**: XAudio2
- **ECS**: EnTT
- **Scripting**: AngelScript (with hot-reload and client/server context separation)
- **Editor**: Dear ImGui (with collaborative multi-user editing)
- **Networking**: UDP client/server, AreaServer/WorldServer architecture (HeroEngine-inspired)
- **Large worlds**: Floating-point origin rebasing, seamless area streaming
- **Headless/Software rendering**: NullRHIDevice fallback (no GPU) or full CPU rendering via OpenGL + Mesa llvmpipe
- **Primary platform**: Windows 10+ (MSVC); Linux/macOS are experimental (macOS has CI job + CMake presets)

## Session start (run at the beginning of every session)

**Step 1 — Git sync** (see [Git Sync Workflow](#git-sync-workflow) below for the commands):

Sync your branch with the latest upstr
```

</details>
