---
name: excalidraw__excalidraw-mcp
source: https://github.com/excalidraw/excalidraw-mcp/blob/157aa23ceb1976008aadc89eb05e3444060f09d6/CLAUDE.md
repo: excalidraw/excalidraw-mcp
kind: claude-md
stars: 4727
last_pushed: 2026-03-24T12:27:09Z
license: unknown
score: 9
domains: [mcp, web-frontend, svg-rendering, typescript]
tags: [mcp-server, excalidraw, streaming-ui, system-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# excalidraw/excalidraw-mcp — claude-md

**Why it's worth keeping:** It provides critical 'mental models' like progressive element ordering to optimize UI streaming and enforces strict debugging protocols (SDK logging vs. console.log).

**Summary:** A highly technical architectural guide for an Excalidraw MCP server featuring SVG streaming, checkpointing, and specialized tool-calling patterns.

**Source credibility:** High; 4.7k stars indicates a widely recognized, high-quality tool in the MCP ecosystem.

**Recency:** Current; pushed 3 months ago, highly relevant to modern MCP development.

**Source:** [excalidraw/excalidraw-mcp/CLAUDE.md](https://github.com/excalidraw/excalidraw-mcp/blob/157aa23ceb1976008aadc89eb05e3444060f09d6/CLAUDE.md) · 4727★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Excalidraw MCP App Server

Standalone MCP server that streams Excalidraw diagrams as SVG with hand-drawn animations.

## Architecture

```
server.ts          → 2 tools (read_me, create_view) + resource + cheat sheet
main.ts            → HTTP (Streamable) + stdio transports
src/mcp-app.tsx    → ExcalidrawAppCore (widget logic) + ExcalidrawApp (useApp wrapper)
src/mcp-entry.tsx  → Production entry point: createRoot + ExcalidrawApp
src/global.css     → Animations (stroke draw-on, fade-in) + auto-resize
src/dev.tsx        → Dev entry point: mock app + sample elements + control panel
src/dev-mock.ts    → Mock MCP App with event simulation (sendToolInput, streamElements, etc.)
index-dev.html     → Dev HTML entry (served by vite dev server)
vite.config.dev.ts → Dev-only vite config (resolves from node_modules, no esm.sh externals)
```

## Tools

### `read_me` (text tool, no UI)
Returns a cheat sheet with element format, color palettes, coordinate tips, and examples. The model should call this before `create_view`.

### `create_view` (UI tool)
Takes `elements` — a JSON string of standard Excalidraw elements. The widget parses partial JSON during streaming and renders via `exportToSvg` +
```

</details>
