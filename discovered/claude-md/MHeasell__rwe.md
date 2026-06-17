---
name: MHeasell__rwe
source: https://github.com/MHeasell/rwe/blob/b2d8a314b14142d8873400160768777532b1dcab/CLAUDE.md
repo: MHeasell/rwe
kind: claude-md
stars: 121
last_pushed: 2026-03-25T23:34:42Z
license: gpl-3.0
score: 9
domains: [game-engine, cpp, typescript, systems-programming]
tags: [build-instructions, architecture-mapping, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# MHeasell/rwe — claude-md

**Why it's worth keeping:** It uses functional descriptions of subdirectories to guide AI code discovery and defines idiomatic patterns like 'Result<T, E>' error handling to ensure consistency.

**Summary:** Provides highly granular build instructions for a hybrid C++/TypeScript project and maps complex engine subsystems to specific directories.

**Source credibility:** High; the file reflects a professionally structured, well-maintained open-source game engine.

**Recency:** Current; follows modern best practices for providing context to AI coding agents.

**Source:** [MHeasell/rwe/CLAUDE.md](https://github.com/MHeasell/rwe/blob/b2d8a314b14142d8873400160768777532b1dcab/CLAUDE.md) · 121★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Robot War Engine (RWE) is an open-source real-time strategy game engine with high compatibility for Total Annihilation data files. It consists of a C++17 core engine and a TypeScript/Electron launcher application. Active priority is simplifying dependencies and improving new developer onboarding.

## Build Commands

### C++ Engine (from repo root)

```bash
# First time setup (submodules + protobuf)
git submodule update --init --recursive
cd libs && ./build-protobuf.sh && cd ..

# Build (Linux/macOS)
mkdir build && cd build
cmake .. -G 'Unix Makefiles' -DCMAKE_BUILD_TYPE=Debug
make -j$(nproc)

# Run unit tests
./build/rwe_test

# Run a single test by name (Catch2 syntax)
./build/rwe_test "test name pattern"
./build/rwe_test "[tag]"
```

### Launcher (from `launcher/` directory)

```bash
npm ci
npm run tsc          # Type check
npm test             # Jest tests
npm run lint         # ESLint
npm run server       # Webpack dev server (hot reload)
npm start            # Launch Electron app (needs RWE_HOME env var)
npm run master-server # Local multipl
```

</details>
