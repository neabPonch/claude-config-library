---
name: Animation-Lab__ProteinBlender
source: https://github.com/Animation-Lab/ProteinBlender/blob/dd9af510e915eca554dc8da3b69cf7e0f834ea10/CLAUDE.md
repo: Animation-Lab/ProteinBlender
kind: claude-md
stars: 25
last_pushed: 2026-06-15T05:26:52Z
license: unknown
score: 9
domains: [graphics-tools, python, blender-addon]
tags: [blender, api-integration, software-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# Animation-Lab/ProteinBlender — claude-md

**Why it's worth keeping:** Uses 'Common Development Tasks' to provide exact coding recipes/patterns and defines data structures/schemas necessary for the agent to write correct logic without guessing the API.

**Summary:** Provides specific context for a complex Blender addon workflow, including environment-specific dependencies and registration patterns.

**Source credibility:** High; active development with clear, technical documentation of a specialized tool.

**Recency:** Very current; includes modern Blender versions and mentions MCP access.

**Source:** [Animation-Lab/ProteinBlender/CLAUDE.md](https://github.com/Animation-Lab/ProteinBlender/blob/dd9af510e915eca554dc8da3b69cf7e0f834ea10/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ProteinBlender is a Blender addon for visualizing and animating protein structures. It integrates MolecularNodes functionality and provides a comprehensive UI for working with molecular data in Blender.

## Development Setup

### Prerequisites
- Blender 4.2 or higher (including Blender 5.0)
- Python 3.11 (matching Blender's Python version)
- You must use Blender's Python environment to test and build code
- VS Code (recommended) with Blender extension
- For development user Windows PowerShell when running commands

### Environment Variables
- `BLENDER_PATH`: Path to Blender executable (required for build.py)

### Key Commands

```bash
# Build the addon package
python build.py

# Development mode - register addon without installing
blender --python dev_register.py

# VS Code tasks available:
# - "Dev: Register Addon" (Ctrl+Shift+B)
# - "Build: Package Addon"
```

## Architecture

### Core Structure
- `__init__.py`: Main addon registration and lifecycle management
- `operators/`: All Blender operators (add molecules, keyframes, etc.)
- `panels/`: U
```

</details>
