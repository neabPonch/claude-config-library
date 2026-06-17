---
name: ford442__brain_viz
source: https://github.com/ford442/brain_viz/blob/0ee9dedf207d1d90568ca615b2d090cb7b8feae8/CLAUDE.md
repo: ford442/brain_viz
kind: claude-md
stars: 3
last_pushed: 2026-06-15T14:35:41Z
license: unknown
score: 9
domains: [graphics, webgpu, data-visualization]
tags: [webgpu, wgsl, low-level, math]
curated: 2026-06-15
curated_by: config-scout
---

# ford442/brain_viz — claude-md

**Why it's worth keeping:** Uses 'negative constraints' to stop the AI from fixing non-standard matrix multiplication and includes precise protocols for updating manual GPU memory offsets.

**Summary:** Provides highly specific technical constraints for WebGPU rendering, focusing on memory alignment and preventing incorrect refactors of custom math logic.

**Source credibility:** Active personal project with recent maintenance.

**Recency:** 

**Source:** [ford442/brain_viz/CLAUDE.md](https://github.com/ford442/brain_viz/blob/0ee9dedf207d1d90568ca615b2d090cb7b8feae8/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Quick Commands

```bash
npm install              # Install dependencies
npm run dev             # Start dev server (http://localhost:5173)
npm run build           # Build production bundle to dist/
npm run preview         # Preview production build locally
python test_run.py      # Smoke test (checks if server responds)
```

## Project Overview

**Neuro-Weaver** is a high-performance 3D volumetric brain visualization engine built with WebGPU and WGSL. It renders stylized brain animations driven by tensor data, supporting multiple visualization styles (Organic surface, Cyber wireframe, Connectome fibers, Heatmap thermal).

**Key tech:** Vanilla JavaScript (ES Modules, no TypeScript), WebGPU graphics API, WGSL compute/rendering shaders, Vite build tool.

## Architecture & Core Components

### Main Modules
- **`main.js`** — Application bootstrap. Initializes BrainRenderer, wires DOM controls, keyboard shortcuts, and runs the main update loop.
- **`brain-renderer.js`** — Core rendering engine. Manages WebGPU device/context, pipelines (render and compute), camera contr
```

</details>
