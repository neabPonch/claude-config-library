---
name: JulNadeauCA__libagar
source: https://github.com/JulNadeauCA/libagar/blob/46e5cd65939dab437f59a3325a0fc0e38fcb36a7/CLAUDE.md
repo: JulNadeauCA/libagar
kind: claude-md
stars: 450
last_pushed: 2026-05-08T01:42:22Z
license: bsd-2-clause
score: 9
domains: [systems-programming, graphics-engine]
tags: [build-system-reference, architectural-patterns, c-language]
curated: 2026-06-15
curated_by: config-scout
---

# JulNadeauCA/libagar — claude-md

**Why it's worth keeping:** It includes a highly useful build system comparison table and explicitly explains how to interact with its custom object-oriented architecture. This allows Claude to write code that adheres to project patterns rather than generic C patterns.

**Summary:** A comprehensive technical reference providing detailed build system workflows and deep semantic context for the toolkit's custom C object/event systems.

**Source credibility:** High; the repository is well-starred (450) and actively maintained.

**Recency:** Very current, reflecting modern build standards like Meson/Ninja.

**Source:** [JulNadeauCA/libagar/CLAUDE.md](https://github.com/JulNadeauCA/libagar/blob/46e5cd65939dab437f59a3325a0fc0e38fcb36a7/CLAUDE.md) · 450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LibAgar is a cross-platform GUI toolkit and application framework written in C. It provides a modular architecture with multiple libraries:

- **CORE**: Platform abstraction, I/O, object system (non-graphical)
- **GUI**: Base framework and standard widgets
- **MATH**: Matrices, vectors, advanced rendering methods
- **NET**: Network interface, HTTP application server
- **VG**: Vector graphics library
- **AU**: Audio interface library
- **SG**: General-purpose 3D engine
- **SK**: Sketches with constraints
- **MAP**: Tile engine

## Build System

LibAgar supports three build systems. See [MESON.md](MESON.md) for detailed Meson documentation.

### 1. BSDBuild
The traditional build system using Autoconf-style configuration:

```bash
./configure --help                    # View all options
./configure --enable-debug            # Debug build with type-safety checks
./configure --prefix=$HOME            # Custom install location
make depend all                       # Build with dependencies
make install                          # Install (may need sudo)
```

</details>
