---
name: rianadon__Cosmos-Keyboards
source: https://github.com/rianadon/Cosmos-Keyboards/blob/ae44f71213b467bf014e5b7ce11bb26de3585191/CLAUDE.md
repo: rianadon/Cosmos-Keyboards
kind: claude-md
stars: 641
last_pushed: 2026-06-09T05:47:25Z
license: agpl-3.0
score: 9
domains: [web-frontend, 3d-graphics, cad-tools]
tags: [sveltekit, threejs, architecture-map, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# rianadon/Cosmos-Keyboards — claude-md

**Why it's worth keeping:** The 'Things that will trip you up' and 'Rendering pipeline' sections provide elite guardrails, preventing the agent from attempting to edit generated files or misplacing logic in a multi-stage pipeline.

**Summary:** A high-context blueprint for a complex 3D CAD/SvelteKit project that maps high-level architecture to low-level build requirements.

**Source credibility:** High; 641 stars on GitHub and actively maintained.

**Recency:** 

**Source:** [rianadon/Cosmos-Keyboards/CLAUDE.md](https://github.com/rianadon/Cosmos-Keyboards/blob/ae44f71213b467bf014e5b7ce11bb26de3585191/CLAUDE.md) · 641★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Cosmos Keyboards — Agent Notes

Web-based generator for ergonomic mechanical keyboards. SvelteKit + TypeScript on top of a heavy CAD/3D pipeline (Three.js + Threlte for rendering, replicad/OpenCascade + Manifold for solids, OpenSCAD for keycaps, MediaPipe for hand scanning).

The user-facing app lives at `/beta` (`src/routes/beta`). Most of the interesting logic is in `src/lib/worker/`, which runs in a Web Worker bridged via `comlink`.

## Toolchain

- **Bun is preferred, Node is the fallback.** The `Makefile` detects `bun` and uses it; otherwise it uses `node` with a custom ESM loader (`src/model_gen/register_loader.js`). When in doubt, use Bun — Node mode is harder to debug.
- **Python venv** is used only for docs (`mkdocs`). Created by `make venv`.
- **`.nvmrc`** pins Node v21+. Use that if running without Bun.

## Build flow

```bash
make quickstart        # one-time: install deps, compile protobufs, generate parts/keycaps geometry
make dev               # start vite dev server → http://localhost:5173/beta
npm run check          # svelte-check + tsc — the closest thing to a CI signal locally
npm test               # runs `bun test` against *.test.ts files
make build
```

</details>
