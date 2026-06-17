---
name: VIDA-NYU__TaxiVis
source: https://github.com/VIDA-NYU/TaxiVis/blob/50e912c72620d247a6e966300eea04de5479eafb/CLAUDE.md
repo: VIDA-NYU/TaxiVis
kind: claude-md
stars: 55
last_pushed: 2025-10-23T13:58:55Z
license: bsd-4-clause
score: 9
domains: [computer-graphics, data-visualization, c++]
tags: [qt, opengl, architecture, spatial-query]
curated: 2026-06-15
curated_by: config-scout
---

# VIDA-NYU/TaxiVis — claude-md

**Why it's worth keeping:** It excels at explaining component relationships and the 'why' behind core data structures, which helps an AI reason about complex system state changes rather than just reading code.

**Summary:** Provides a comprehensive architectural map that links high-level logic to specific file paths and data structures.

**Source credibility:** High-quality academic project from NYU (VIDA).

**Recency:** The tech stack is legacy, but the documentation pattern is a gold standard for modern AI coding agents.

**Source:** [VIDA-NYU/TaxiVis/CLAUDE.md](https://github.com/VIDA-NYU/TaxiVis/blob/50e912c72620d247a6e966300eea04de5479eafb/CLAUDE.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

TaxiVis (also referred to as TLCVis) is a Qt4-based visual analytics application for exploring NYC taxi trip data. The application provides interactive visualization of taxi trips using OpenGL rendering, with support for spatial and temporal queries.

## Build System

### Building the Main Application

The project uses CMake (minimum 2.6) as its primary build system:

```bash
cd src/TaxiVis
mkdir build
cd build
cmake ../
make
```

Alternative build with QMake:
```bash
cd src/TaxiVis
qmake
make
```

### Building Preprocessing Tools

Data preprocessing utilities are built separately:

```bash
cd src/preprocess
mkdir build
cd build
cmake ../
make
```

This generates executables: `csv2Binary`, `newFormatCsv2Binary`, `multiCsv2Binary`, `build_kdtrip`, `sampling`, `testQuery`, `unif96_to_bin`.

### Dependencies

- CMake (2.6+)
- Qt 4 (4.8.5+) with QtWebkit and QtOpenGL
- OpenGL/GLEW (1.10.0-3+)
- Boost (1.42+): system, iostreams, filesystem, timer components

## Data Management

### Data Location

- Default data directory: `data/` (relative to reposito
```

</details>
