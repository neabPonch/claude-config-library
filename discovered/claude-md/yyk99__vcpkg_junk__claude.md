---
name: yyk99__vcpkg_junk__claude
source: https://github.com/yyk99/vcpkg_junk/blob/a6a550405f68e0014557a975a161b2dd02d98724/14_vulkan_primer/CLAUDE.md
repo: yyk99/vcpkg_junk
kind: claude-md
stars: 0
last_pushed: 2026-01-23T11:59:21Z
license: unknown
score: 8
domains: [graphics, cpp, vulkan]
tags: [cmake-presets, vulkan, build-system, architectural-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# yyk99/vcpkg_junk — claude-md

**Why it's worth keeping:** Explicitly maps data structures to specific line numbers and provides exact command-line arguments for different OS environments, reducing AI guesswork during build tasks.

**Summary:** Provides precise build instructions using CMake presets and detailed architectural breakdowns of Vulkan rendering stages.

**Source credibility:** Low (repository name suggests experimental/junk status), but the documentation itself is professional and highly structured.

**Recency:** Current; uses modern CMake preset patterns which are ideal for current development workflows.

**Source:** [yyk99/vcpkg_junk/14_vulkan_primer/CLAUDE.md](https://github.com/yyk99/vcpkg_junk/blob/a6a550405f68e0014557a975a161b2dd02d98724/14_vulkan_primer/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Vulkan graphics programming primer project containing three example applications that demonstrate Vulkan API usage with GLFW for window management. The project showcases basic Vulkan initialization, classic triangle rendering with a complete graphics pipeline, and advanced 3D cube rendering.

## Build System

### Dependencies
- vcpkg (package manager)
- CMake 3.10+
- C++17 compiler
- Vulkan SDK
- GLFW3 (via vcpkg)
- GLM (via vcpkg)

### Configuration

**Using CMake Presets (Recommended):**
```bash
# Windows - use one of: default, windows-developmentyk, cherry
cmake --preset=default

# Linux - use kestrel (GCC) or kestrel-clang (Clang)
cmake --preset=kestrel
cmake --preset=kestrel-clang
```

Available presets in CMakeUserPresets.json:
- `default`: Windows (G:\opt\vcpkg)
- `windows-developmentyk`: Windows (C:\opt\vcpkg)
- `cherry`: Windows (E:\opt\vcpkg)
- `kestrel`: Linux with GCC (/home/yyk/src/vcpkg)
- `kestrel-clang`: Linux with Clang (/home/yyk/src/vcpkg)

**Manual Configuration:**
```bash
cmake -S . -B build-vs2022-x64 -DCMAKE_TOOLC
```

</details>
