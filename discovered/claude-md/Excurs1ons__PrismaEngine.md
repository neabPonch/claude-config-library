---
name: Excurs1ons__PrismaEngine
source: https://github.com/Excurs1ons/PrismaEngine/blob/c050fc8a6cb28786ed01f9fa1e7df6cffd249b5e/CLAUDE.md
repo: Excurs1ons/PrismaEngine
kind: claude-md
stars: 1
last_pushed: 2026-06-06T05:07:57Z
license: mit
score: 9
domains: [game-engine, cpp, cross-platform]
tags: [cmake, build-system, architecture, multilingual]
curated: 2026-06-16
curated_by: config-scout
---

# Excurs1ons/PrismaEngine — claude-md

**Why it's worth keeping:** Includes specific environment variable workarounds for platform-specific runtime failures (e.g., .NET memory issues in Termux) and offers highly granular CMake preset commands.

**Summary:** Provides exhaustive cross-platform build instructions and a hierarchical architectural map for a C++23 game engine.

**Source credibility:** Low star count, but content is clearly hand-authored with high technical density.

**Recency:** Very current; references C++23 and modern .NET environments.

**Source:** [Excurs1ons/PrismaEngine/CLAUDE.md](https://github.com/Excurs1ons/PrismaEngine/blob/c050fc8a6cb28786ed01f9fa1e7df6cffd249b5e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Prisma Engine (formerly YAGE - Yet Another Game Engine) is a cross-platform game engine built with modern C++23. It supports Windows, Linux, and Android platforms with a focus on modern graphics APIs (DirectX 12, Vulkan).

## 项目概述 / Project Overview (Chinese)

Prisma Engine（原 YAGE - Yet Another Game Engine）是一个使用现代 C++23 构建的跨平台游戏引擎。支持 Windows、Linux 和 Android 平台，专注于现代图形 API（DirectX 12、Vulkan）。

## Build Commands

### Windows Builds
Using CMake presets (recommended):
```bash
# 1. Configure (creates Visual Studio solution in build/windows-x64-debug)
cmake --preset windows-x64-debug

# 2. Build all targets (from the build directory directly)
cmake --build build/windows-x64-debug

# Or build specific targets only
cmake --build build/windows-x64-debug --target Engine
cmake --build build/windows-x64-debug --target Editor
cmake --build build/windows-x64-debug --target Launcher
cmake --build build/windows-x64-debug --target PathTracing3D

# Release
cmake --preset windows-x64-release
cmake --build build/windows-x64-release
```

Using Visual Studio:
1. Open
```

</details>
