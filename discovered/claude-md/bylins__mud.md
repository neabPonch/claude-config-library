---
name: bylins__mud
source: https://github.com/bylins/mud/blob/9fe683f547daed0e0ed30bc42ccf9bdf4392e917/CLAUDE.md
repo: bylins/mud
kind: claude-md
stars: 41
last_pushed: 2026-06-16T14:09:35Z
license: other
score: 9
domains: [game-engine, systems-programming, cpp]
tags: [meson, build-system, architecture-mapping, game-dev]
curated: 2026-06-16
curated_by: config-scout
---

# bylins/mud — claude-md

**Why it's worth keeping:** The 'CRITICAL' warnings regarding execution directories prevent AI from making common runtime path errors, while the detailed architecture section provides excellent context for where logic resides.

**Summary:** A high-quality technical manual for a complex C++20 game engine that prioritizes correct execution paths and build profiles. It maps out specific architectural patterns like the pulse-based loop and entity hierarchy.

**Source credibility:** Legitimate project with growing popularity (41 stars) and active maintenance.

**Recency:** Very recent; utilizes modern standards like C++20 and Meson/Ninja build systems.

**Source:** [bylins/mud/CLAUDE.md](https://github.com/bylins/mud/blob/9fe683f547daed0e0ed30bc42ccf9bdf4392e917/CLAUDE.md) · 41★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is **Bylins MUD** - a Russian-language Multi-User Dungeon game server based on CircleMUD/DikuMUD. The codebase is ~272K lines of C++20 code with extensive Russian comments and variable names. It implements a complete multiplayer text-based RPG with combat, magic, crafting, quests, and scripting systems.

## Build Commands

### Initial Setup (Ubuntu/WSL)
```bash
sudo apt update && sudo apt upgrade
sudo apt install build-essential meson ninja-build libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext unzip gdb libgtest-dev zlib1g-dev
git clone --recurse-submodules https://github.com/bylins/mud
cd mud
cp -n -r lib.template/* lib
```

### Если репозиторий уже склонирован без submodules

```bash
git submodule update --init --recurse-submodules
```

### Standard Build (without tests)
```bash
meson setup build -Dbuild_tests=false -Dbuild_profile=release
ninja -C build -j$(($(nproc)/2))
./build/circle 4000  # Start server on port 4000
```

### Build with Tests
```bash
meson setup build -Dbuild_profile=release -Dbuild_tests=true
ninja -C build -j$(($
```

</details>
