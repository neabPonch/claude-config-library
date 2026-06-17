---
name: Tac213__im-neovim
source: https://github.com/Tac213/im-neovim/blob/6a6ac5ce8f67dd6544d0de75852acd700a6574d0/CLAUDE.md
repo: Tac213/im-neovim
kind: claude-md
stars: 0
last_pushed: 2026-06-14T12:05:42Z
license: apache-2.0
score: 9
domains: [c-plus-plus, desktop-app, cross-platform]
tags: [architecture, build-instructions, style-guide]
curated: 2026-06-15
curated_by: config-scout
---

# Tac213/im-neovim — claude-md

**Why it's worth keeping:** It includes detailed architectural explanations of custom patterns to prevent AI hallucination and a comprehensive naming convention table for style compliance.

**Summary:** A high-quality technical manual that explains not just where files are, but how specific internal systems (Signal/Slot and Asset management) operate.

**Source credibility:** The repository has low social proof (0 stars), but the documentation quality suggests a professional-grade C++ codebase.

**Recency:** Very current, explicitly mentioning 'claude.ai/code' and modern build workflows.

**Source:** [Tac213/im-neovim/CLAUDE.md](https://github.com/Tac213/im-neovim/blob/6a6ac5ce8f67dd6544d0de75852acd700a6574d0/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
```
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ImNeovim is an ImGui-based graphical user interface for Neovim. It embeds Neovim and provides a modern, customizable UI using ImGui, with support for multiple platforms (Windows, Linux, macOS) and graphics backends (OpenGL, DirectX 12, Metal).

## Repository Structure

```

├── src/
│ ├── im_app/ # Core application framework (cross-platform)
│ │ ├── interfaces/ # Abstract interfaces for graphics, window, renderer
│ │ ├── platforms/ # Platform-specific implementations
│ │ │ ├── win32/ # Windows implementation
│ │ │ ├── linux/ # Linux implementation (GLFW-based)
│ │ │ └── darwin/ # macOS implementation
│ │ └── application.cpp # Main application logic
│ └── im_neovim/ # Neovim integration
│ ├── include/ # Private headers
│ ├── gui/ # GUI widgets (text_widget, terminal, nvim_widget)
│ ├── layers/ # Layer implementations (libuv)
│ └── im_neovim_app.cpp # Main entry point for ImNeovim
├── include/
│ └── im_app/ # Public API headers
├── thirdparty/ # Submodules and dependencies
│ ├── imgui/ # ImGui library
│ ├── glfw/ # GLFW window library (Linux/ma
```

</details>
