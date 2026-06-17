---
name: DingoOz__BranchForge
source: https://github.com/DingoOz/BranchForge/blob/05584dcca5ea4a9c894ac7a6b73b1958ed11b1c6/CLAUDE.md
repo: DingoOz/BranchForge
kind: claude-md
stars: 1
last_pushed: 2025-12-31T08:34:44Z
license: mit
score: 9
domains: [robotics, cpp-qt, desktop-apps]
tags: [cmake, qt6, ros2, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# DingoOz/BranchForge — claude-md

**Why it's worth keeping:** The 'Data Flow' section and the QML-C++ bridge mapping provide essential context that prevents architectural hallucination. It also includes specific, actionable build/test command sequences.

**Summary:** A highly structured guide for a C++/Qt robotics tool, detailing build commands, component responsibilities, and complex data flows.

**Source credibility:** Low star count (1), but the technical depth suggests a high-quality individual project.

**Recency:** Recent; utilizes modern C++20 and Qt6 standards relevant to current development environments.

**Source:** [DingoOz/BranchForge/CLAUDE.md](https://github.com/DingoOz/BranchForge/blob/05584dcca5ea4a9c894ac7a6b73b1958ed11b1c6/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

BranchForge is an open-source development platform for designing, visualizing, testing, and debugging Behaviour Trees (BTs) for ROS2 robotics applications. Built with C++20 and Qt6 QML on Ubuntu.

## Build Commands

```bash
# Build (from project root)
mkdir -p build && cd build && cmake .. && make -j$(nproc)

# Run the application
./build/branchforge_enhanced

# Build with tests
cmake -DBUILD_TESTING=ON .. && make -j$(nproc)

# Run all tests
ctest

# Run a specific test
./build/tests/unit/test_behavior_tree_xml

# Run tests with verbose output
ctest --verbose
```

## Dependencies

```bash
# Qt6 (required)
sudo apt install -y qt6-base-dev qt6-declarative-dev qt6-quick3d-dev

# Build tools
sudo apt install -y cmake build-essential pkg-config

# Testing (optional)
sudo apt install -y libgtest-dev
```

## Architecture

### Application Startup Flow
1. `src/main.cpp` → Creates `Application` instance
2. `src/core/Application.cpp` → Initializes Qt, registers QML types, loads QML engine
3. `qml/main.qml` → Main window with three-panel SplitView layout
4.
```

</details>
