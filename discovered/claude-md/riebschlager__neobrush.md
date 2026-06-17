---
name: riebschlager__neobrush
source: https://github.com/riebschlager/neobrush/blob/e1925562d732f05afef88749466ab0b2264fbaac/CLAUDE.md
repo: riebschlager/neobrush
kind: claude-md
stars: 84
last_pushed: 2026-01-05T05:53:13Z
license: unknown
score: 8
domains: [web-frontend, creative-coding]
tags: [vue-3, typescript, architecture, canvas]
curated: 2026-06-15
curated_by: config-scout
---

# riebschlager/neobrush — claude-md

**Why it's worth keeping:** It uses 'Architecture' sections to explain complex logic (physics/rendering) rather than just listing files, providing the LLM with a mental model of how algorithms interact.

**Summary:** A high-quality instruction file that defines a generative art engine using Vue 3 and TypeScript.

**Source credibility:** A moderately-starred GitHub repository from a niche generative art project.

**Recency:** Current; utilizes modern tech stacks like Vue 3 and Vite.

**Source:** [riebschlager/neobrush/CLAUDE.md](https://github.com/riebschlager/neobrush/blob/e1925562d732f05afef88749466ab0b2264fbaac/CLAUDE.md) · 84★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NeoBrush is a modern Vue 3 + TypeScript generative art application with an Adobe Creative Suite-inspired interface. It creates organic, flowing brush strokes using physics-based vertex animation that samples colors from source images.

**Tech Stack:** Vue 3, Vite, TypeScript, Vuetify 3 (dark theme), Pinia, Canvas 2D API

## Commands

```bash
npm run dev      # Start development server
npm run build    # Build for production (includes type checking)
npm run preview  # Preview production build
```

## Project Structure

```
src/
├── components/
│   ├── canvas/         # CanvasViewport - main drawing surface
│   ├── panels/         # ToolsPanel, PropertiesPanel, LayersPanel
│   └── common/         # MenuBar, StatusBar
├── composables/        # useNeoBrush - connects engine to Vue
├── engine/             # Framework-agnostic rendering engine
│   ├── brushes/        # NeoBrush, SketchLine classes
│   └── core/           # CanvasManager, Vector2D
├── stores/             # Pinia stores (brush, canvas, layers, history)
├── types/              # TypeScrip
```

</details>
