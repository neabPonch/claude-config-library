---
name: karlforshaw__offblast
source: https://github.com/karlforshaw/offblast/blob/f5fa63cb122b5c6cf116a29c1100cc07e71b56a9/CLAUDE.md
repo: karlforshaw/offblast
kind: claude-md
stars: 18
last_pushed: 2026-06-14T21:08:54Z
license: gpl-3.0
score: 7
domains: [cli-tools, game-dev, c-programming]
tags: [architecture-mapping, build-instructions, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# karlforshaw/offblast — claude-md

**Why it's worth keeping:** It provides a clear mental model of the application's data hierarchy (e.g., specifying where LaunchTarget resides), which is crucial for LLMs working in low-level C projects.

**Summary:** A structured architectural overview that maps core data structures, dependencies, and platform-specific logic to specific files.

**Source credibility:** A specialized niche project; note the likely typo regarding 'main.c' line counts which may impact accuracy.

**Recency:** Current and highly compatible with Claude Code's context requirements.

**Source:** [karlforshaw/offblast/CLAUDE.md](https://github.com/karlforshaw/offblast/blob/f5fa63cb122b5c6cf116a29c1100cc07e71b56a9/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

- **Build**: `make`
- **Clean**: `make clean`
- **Install config**: `make install` (creates ~/.offblast/config.json from config-dist.json)
- **Run**: `./offblast`

## Codebase Overview

OffBlast is a game launcher written in C using SDL2 and OpenGL. The project consists of a single main executable that provides a visual interface for launching games through various emulators and launchers.

### Key Components

- **main.c** (181K lines): Core application logic including UI rendering, input handling, game database management, and launcher integration
- **offblastDbFile.c/h**: Database file format handling for storing game metadata, launcher configs, and playtime tracking
- **shaders/**: GLSL shaders for rendering UI elements (text, images, gradients)

### Platform Support

The launcher supports multiple platforms through different launcher types:
- **retroarch**: Generic RetroArch launcher for various console platforms
- **cemu**: Wii U emulator support
- **dolphin**: GameCube emulator (via custom launcher)
- **pcsx2**: PlayStation 2 emulator
- **rpc
```

</details>
