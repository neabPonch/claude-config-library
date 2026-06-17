---
name: lewish__asciiflow
source: https://github.com/lewish/asciiflow/blob/459cbadd679358cdba42f557c689c4b508bfef32/CLAUDE.md
repo: lewish/asciiflow
kind: claude-md
stars: 5751
last_pushed: 2026-04-23T01:33:01Z
license: mit
score: 9
domains: [web-frontend, desktop-app]
tags: [architecture-heavy, comprehensive-documentation]
curated: 2026-06-17
curated_by: config-scout
---

# lewish/asciiflow — claude-md

**Why it's worth keeping:** It explains complex design patterns (Command pattern/Zustand) rather than just listing files, and the inclusion of a prioritized issue list provides crucial semantic context for current development goals.

**Summary:** A highly detailed technical reference covering build systems, architectural patterns, and project-wide conventions.

**Source credibility:** High; popular repository with significant star count and recent activity.

**Recency:** Very current; uses modern toolchains like Node 22 and Bazel 8.

**Source:** [lewish/asciiflow/CLAUDE.md](https://github.com/lewish/asciiflow/blob/459cbadd679358cdba42f557c689c4b508bfef32/CLAUDE.md) · 5751★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ASCIIFlow

ASCII diagram drawing web app (asciiflow.com). Client-side only, also runs as Electron desktop app.

## Stack

- **Language:** TypeScript 5.8
- **UI:** React 16.14.0 + Material-UI 4.12.4
- **Routing:** React Router DOM 5.3.4
- **Build:** Bazel 8 (via Bazelisk) + esbuild (via aspect_rules_esbuild)
- **Tests:** Mocha + Chai + Sinon (unit), Playwright (e2e)
- **Desktop:** Electron 29.0.1

## Build & Dev

```bash
bazel build client:bundle      # Production build (esbuild)
bazel build client:site         # Full site with static assets
bazel test //common:all         # Common tests only
bazel test //client:all         # Client tests only
bazel test //e2e:all            # Playwright e2e tests
```

Requires Node 22.x (managed by Bazel toolchain) and Bazel 8.x (via Bazelisk).

## Project Structure

```
client/                # Main frontend app
  store/               # State management (Zustand)
    index.ts           # Store singleton, ToolMode enum, tool instances
    canvas.ts          # Per-drawing state (layers, undo/redo, zoom)
    drawing_stringifier.ts  # Compress/share drawings via URL
  draw/                # Drawing tool implementations (IDrawFunction interface)
```

</details>
