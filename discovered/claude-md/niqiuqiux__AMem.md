---
name: niqiuqiux__AMem
source: https://github.com/niqiuqiux/AMem/blob/94092d661b74d0f707e4ea37056a762834421eeb/CLAUDE.md
repo: niqiuqiux/AMem
kind: claude-md
stars: 85
last_pushed: 2026-05-29T18:36:55Z
license: gpl-2.0
score: 9
domains: [desktop-apps, systems-programming]
tags: [c-plus-plus, windows, cmake, multithreading]
curated: 2026-06-17
curated_by: config-scout
---

# niqiuqiux/AMem — claude-md

**Why it's worth keeping:** The 'Key Patterns' section is exceptional, explicitly detailing thread-safety requirements for socket communication and singleton patterns that an AI needs to avoid breaking system state.

**Summary:** Provides high-fidelity build instructions, dependency management, and a deep architectural breakdown of the C++ project.

**Source credibility:** Solid mid-sized open source project with recent activity and specific technical requirements.

**Recency:** Very current; follows modern C++/CMake standards useful for today's Claude Code.

**Source:** [niqiuqiux/AMem/CLAUDE.md](https://github.com/niqiuqiux/AMem/blob/94092d661b74d0f707e4ea37056a762834421eeb/CLAUDE.md) · 85★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AMem is a Windows desktop application for remote Android memory debugging, similar to Cheat Engine. It connects to an Android device over Socket and provides memory scanning, hardware breakpoint debugging, and a hex memory viewer. The UI is built with Dear ImGui (docking branch) rendered via DirectX 12.

Language: C++17. Platform: Windows 10/11 x64 only.

## Build Commands

```bash
# Configure (from repo root)
cmake -B build -G "Visual Studio 17 2022" -A x64

# Build Release
cmake --build build --config Release

# Build Debug
cmake --build build --config Debug
```

Output binary: `bin/ImGuiProject.exe`

The project can also be opened directly in Visual Studio via CMakeLists.txt (select x64-Release or x64-Debug).

## Dependencies

- **Required**: Visual Studio 2022 (C++17), CMake 3.16+, DirectX 12 SDK, Windows SDK
- **Required**: LuaJIT — must be placed in `third_party/LuaJIT/` with `include/` and `lib/lua51.lib`
- **Optional**: Capstone disassembly library — enables disassembly features in breakpoint window. Install via `vcpkg install capstone:x6
```

</details>
