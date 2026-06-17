---
name: LuaLanes__lanes
source: https://github.com/LuaLanes/lanes/blob/4aa54c9a6876c4af175b306fffe8dbc010e72c5b/CLAUDE.md
repo: LuaLanes/lanes
kind: claude-md
stars: 534
last_pushed: 2026-03-12T10:21:59Z
license: other
score: 10
domains: [systems-programming, lua, cpp, multithreading]
tags: [build-instructions, architecture-mapping, style-guide, testing-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# LuaLanes/lanes — claude-md

**Why it's worth keeping:** It maps high-level architecture to specific files and explains complex data flows (e.s. Send/Receive) which is vital for LLM reasoning. The inclusion of an explicit, tabular naming convention prevents stylistic drift in system-level code.

**Summary:** A masterclass in providing architectural context, detailed build/test workflows, and strict coding conventions for a hybrid C++/Lua project.

**Source credibility:** High; a well-starred (534), active, and professionally structured systems library.

**Recency:** Highly current, referencing modern C++20 standards and recent macOS deployment targets.

**Source:** [LuaLanes/lanes/CLAUDE.md](https://github.com/LuaLanes/lanes/blob/4aa54c9a6876c4af175b306fffe8dbc010e72c5b/CLAUDE.md) · 534★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Lua Lanes is a portable, message-passing multithreading library for Lua, implemented as a C++20 shared library (`lanes_core.dll/.so`) with a Lua wrapper (`lanes.lua`). It allows running multiple independent Lua states in parallel threads. Supported Lua versions: 5.1, 5.2, 5.3, 5.4, 5.5, and LuaJIT.

## Build Commands

The primary build system is GNU Make (MSYS/MinGW on Windows). There is also a Visual Studio solution (`Lanes.sln`) and a `CMakeLists.txt`.

```bash
# Build lanes_core shared library only (default)
make

# Build C++ unit tests
make build_unit_tests

# Build deep_userdata_example side module
make build_DUE

# Build and run all unit tests
make run_unit_tests

# Debug build (unoptimized)
make debug

# Clean all build artifacts
make clean

# LuaRocks build
luarocks make
```

On Mac OS X, building requires explicit C++20 flags:
```bash
luarocks make CC="env MACOSX_DEPLOYMENT_TARGET=13.3 gcc" LD="env MACOSX_DEPLOYMENT_TARGET=13.3 gcc" CFLAGS="-O2 -fPIC -std=c++20"
```

## Running Tests

### Integration tests (Lua scripts in `tests/`)
```bash
#
```

</details>
