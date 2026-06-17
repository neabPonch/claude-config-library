---
name: ytliu74__obsidian-pseudocode
source: https://github.com/ytliu74/obsidian-pseudocode/blob/5ace9075dbe50bc1c64ee1d6e0bc228f3cb64591/CLAUDE.md
repo: ytliu74/obsidian-pseudocode
kind: claude-md
stars: 134
last_pushed: 2026-05-06T01:01:09Z
license: mit
score: 9
domains: [obsidian-plugin, typescript, web-extension]
tags: [architecture-mapping, logic-flow, implementation-details]
curated: 2026-06-15
curated_by: config-scout
---

# ytliu74/obsidian-pseudocode — claude-md

**Why it's worth keeping:** The 'Core Processing Flow' sequence and the 'Important Implementation Details' section provide high-level logic that isn't easily inferred from code alone. It bridges the gap between file structure and actual runtime behavior.

**Summary:** This file provides a highly detailed architectural map including logical processing flows and critical implementation nuances.

**Source credibility:** Solid; 134 stars indicates a functional, community-vetted tool.

**Recency:** Current; aligns with modern TypeScript/esbuild development workflows.

**Source:** [ytliu74/obsidian-pseudocode/CLAUDE.md](https://github.com/ytliu74/obsidian-pseudocode/blob/5ace9075dbe50bc1c64ee1d6e0bc228f3cb64591/CLAUDE.md) · 134★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Obsidian-Pseudocode is an Obsidian plugin that renders LaTeX-style pseudocode inside code blocks. It uses pseudocode.js to convert LaTeX algorithmic constructs to HTML, with support for math formulas via KaTeX.

## Build and Development Commands

```bash
# Development mode with file watching
npm run dev

# Production build (includes TypeScript type checking)
npm run build

# Version bump
npm run version
```

## Architecture

### Plugin Entry Point
- `main.ts`: Core plugin class (`PseudocodePlugin`)
  - Registers markdown code block processor for `pseudo` language
  - Manages settings and preamble loading
  - Handles theme observer lifecycle

### Core Processing Flow
1. User creates a code block with `pseudo` language specifier
2. `pseudocodeHandler()` in main.ts processes the block:
   - Extracts inline macros (before `\begin{algorithm}`)
   - Combines with global preamble if enabled
   - Injects preamble into all math expressions (`$...$`)
   - Renders using pseudocode.js library
   - Adds export button and applies theme

### Key Modules

**src/
```

</details>
