---
name: Devinci297__MSFS-LOD-Maker
source: https://github.com/Devinci297/MSFS-LOD-Maker/blob/11cf0fd166815e4d33a771cb83a6c06621f85041/CLAUDE.md
repo: Devinci297/MSFS-LOD-Maker
kind: claude-md
stars: 8
last_pushed: 2026-02-19T15:53:04Z
license: mit
score: 8
domains: [3d-tooling, game-dev, blender]
tags: [pipeline-logic, domain-specific, workflow-oriented]
curated: 2026-06-15
curated_by: config-scout
---

# Devinci297/MSFS-LOD-Maker — claude-md

**Why it's worth keeping:** Excellent use of 'Pipeline' documentation to explain data flow transformations and explicit domain rules (naming patterns/vertex modes) that are not obvious from code alone.

**Summary:** Provides a clear architectural breakdown of a specific logic pipeline and detailed manual workflows for non-CLI development.

**Source credibility:** Low star count, but high-quality, structured content suggests a professional developer workflow.

**Recency:** Very recent; fully compatible with modern Claude Code needs.

**Source:** [Devinci297/MSFS-LOD-Maker/CLAUDE.md](https://github.com/Devinci297/MSFS-LOD-Maker/blob/11cf0fd166815e4d33a771cb83a6c06621f85041/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Blender addon for Microsoft Flight Simulator (MSFS) LOD (Level of Detail) generation. The addon creates multiple LOD levels from a base collection using various optimization methods, with automatic LOD value calculation based on MSFS 2024 standards.

## Architecture

The addon follows standard Blender addon structure with 4 main components:

- **`__init__.py`** - Addon registration and metadata
- **`operators.py`** - Core LOD generation logic and operators
- **`properties.py`** - Property definitions and scene data
- **`ui.py`** - User interface panels and lists

### Key Components

**LOD Generation Pipeline:**
1. Find active LOD00 collections (collections ending with "_LOD00")
2. Calculate object size and optimal LOD values
3. Generate LOD01-03 collections using configurable methods
4. Apply vertex colors and modifiers
5. Integrate with MSFS Multi-Export addon

**Generation Methods:**
- **Mixed (default)**: Decimate modifier for all LODs (LOD01-03)
- **Decimate Only**: Decimate modifier for all LODs
- **Shrinkwrap Only**: Cube proxy with shrin
```

</details>
