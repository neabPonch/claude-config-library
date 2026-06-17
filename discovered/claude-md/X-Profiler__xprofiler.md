---
name: X-Profiler__xprofiler
source: https://github.com/X-Profiler/xprofiler/blob/fd66e7f4a0770aaf12cea4c6f9a44ad52090a43d/CLAUDE.md
repo: X-Profiler/xprofiler
kind: claude-md
stars: 451
last_pushed: 2026-04-22T08:08:10Z
license: other
score: 9
domains: [node-js, systems-programming, performance-monitoring, cli-tools]
tags: [native-addon, multi-threading, build-system, profiling]
curated: 2026-06-14
curated_by: config-scout
---

# X-Profiler/xprofiler — claude-md

**Why it's worth keeping:** The 'Common Development Tasks' section provides perfect procedural recipes for extending the project, while the threading and platform-specific notes prevent critical low-level errors.

**Summary:** A highly detailed technical guide for a Node.js native addon that covers build systems, multi-threaded architecture, and platform-specific nuances.

**Source credibility:** High; a well-starred (451) performance tool with recent maintenance activity.

**Recency:** Current; includes specific details regarding Node.js v24 and modern C++ standards.

**Source:** [X-Profiler/xprofiler/CLAUDE.md](https://github.com/X-Profiler/xprofiler/blob/fd66e7f4a0770aaf12cea4c6f9a44ad52090a43d/CLAUDE.md) · 451★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

X-Profiler is a Node.js native addon for runtime profiling and performance monitoring. It outputs performance logs at regular intervals and enables real-time runtime state sampling via external commands (xprofctl CLI).

**Supported Platforms:** Windows, Linux (x64/arm64), macOS (x64/arm64)
**Node.js Versions:** v18.x, v20.x, v22.x, v24.x (LTS only)

## Build Commands

```bash
# Build the native addon (requires C++ toolchain)
npm run build

# Build with pre-built binary download (fallback to build from source)
npm install

# Run all tests
npm run test

# Run a single test file
npm run test-single test/config.test.js

# Generate coverage report
npm run cov

# Run coverage for a single test
npm run cov-single test/config.test.js

# Full CI suite (lint + build + coverage)
npm run ci

# Format C++ code (requires clang-format)
npm run format

# Lint JavaScript code
npm run lint
```

## Build System & C++ Compilation

**C++ Standard Requirements:**
- Linux: Uses C++17 (`-std=c++17` in `cflags`)
- macOS: Uses C++20 (`-std=c++20` in `xcode_settings.OTHER_
```

</details>
