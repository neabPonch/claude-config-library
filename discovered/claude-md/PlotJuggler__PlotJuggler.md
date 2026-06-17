---
name: PlotJuggler__PlotJuggler
source: https://github.com/PlotJuggler/PlotJuggler/blob/034a5cc919909aebb124e0dc1abbe2029c3eed0f/CLAUDE.md
repo: PlotJuggler/PlotJuggler
kind: claude-md
stars: 5956
last_pushed: 2026-05-11T12:46:31Z
license: mpl-2.0
score: 9
domains: [cpp, desktop-app, data-visualization]
tags: [qt, cmake, plugin-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# PlotJuggler/PlotJuggler — claude-md

**Why it's worth keeping:** Includes high-value 'tribal knowledge' like unique Plugin IIDs and thread-safety requirements that are critical for LLM-driven extension work. The layered architecture breakdown is highly effective at giving the AI a mental model of the codebase.

**Summary:** Provides comprehensive build/test instructions, architectural layering, and specific plugin interface metadata for a complex C++/Qt application.

**Source credibility:** High; based on a popular, actively maintained open-source tool with nearly 6k stars.

**Recency:** Very current; repository activity within the last month suggests up-to-date build instructions.

**Source:** [PlotJuggler/PlotJuggler/CLAUDE.md](https://github.com/PlotJuggler/PlotJuggler/blob/034a5cc919909aebb124e0dc1abbe2029c3eed0f/CLAUDE.md) · 5956★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PlotJuggler is a Qt5-based C++17 desktop application for visualizing time series data. It supports file loading, real-time streaming, data transformation, and export via a dynamic plugin system. Licensed under MPL-2.0.

## Build Commands

```bash
# Linux (Ubuntu) - install deps first:
# sudo apt -y install qtbase5-dev libqt5svg5-dev libqt5websockets5-dev libqt5serialport5-dev \
#   libqt5opengl5-dev libqt5x11extras5-dev libprotoc-dev libzmq3-dev liblz4-dev libzstd-dev

# Configure and build
cmake -S . -B build -DCMAKE_INSTALL_PREFIX=install
cmake --build build --config RelWithDebInfo --target install

# With Conan (Windows/cross-platform)
conan install . --output-folder build --build missing
cmake -S . -B build -DCMAKE_TOOLCHAIN_FILE=build/conan_toolchain.cmake \
      -DCMAKE_INSTALL_PREFIX=install -DBUILDING_WITH_CONAN=ON
cmake --build build --config RelWithDebInfo --target install

# Run
./build/bin/plotjuggler
```

Key CMake options: `ENABLE_ASAN`, `BASE_AS_SHARED` (ON for ROS2), `BUILDING_WITH_CONAN`, `PJ_PLUGINS_DIRECTORY`.

## Testing

```
```

</details>
