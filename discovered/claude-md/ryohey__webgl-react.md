---
name: ryohey__webgl-react
source: https://github.com/ryohey/webgl-react/blob/20caf456a8b66dfcba8b875e0d7ca159bb0fe1a3/CLAUDE.md
repo: ryohey/webgl-react
kind: claude-md
stars: 18
last_pushed: 2025-11-15T09:51:05Z
license: mit
score: 8
domains: [web-frontend, graphics, library-development]
tags: [react, webgl, architecture, monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# ryohey/webgl-react — claude-md

**Why it's worth keeping:** The 'Rendering Flow' section provides a crucial procedural mental model for how components interact. It also maps high-level concepts directly to specific file paths, reducing AI search time.

**Summary:** Provides a clear command reference for a multi-workspace monorepo and a deep technical overview of the WebGL rendering engine.

**Source credibility:** A niche but well-structured open-source React library.

**Recency:** Current and highly relevant to modern development workflows.

**Source:** [ryohey/webgl-react/CLAUDE.md](https://github.com/ryohey/webgl-react/blob/20caf456a8b66dfcba8b875e0d7ca159bb0fe1a3/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Development
- `npm start` - Start both lib and example development servers concurrently
- `npm run start:lib` - Start lib development server (Rollup watch mode)
- `npm run start:example` - Start example development server (Vite)

### Build and Test
- `npm run build` - Build the library (runs in lib workspace)
- `npm test` - Run tests using Vitest (runs in lib workspace)
- `npm run test:watch` - Run tests in watch mode (in lib workspace)
- `npm publish` - Publish library to npm (runs in lib workspace)

### Workspace Commands
The project uses npm workspaces with two main workspaces:
- `lib/` - The main webgl-react library
- `example/` - Example application demonstrating library usage

## Architecture

### Core Architecture
webgl-react is a React library for high-performance 2D rendering using WebGL with screen coordinates. The library uses a component-based architecture where WebGL rendering is abstracted into React components.

### Key Components

#### GLCanvas (`lib/src/GLCanvas/GLCanvas.tsx`)
- Root WebGL component that initializes WebGL context
- P
```

</details>
