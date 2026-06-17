---
name: walterlow__freecut
source: https://github.com/walterlow/freecut/blob/fe595df738ffaf07713dd825b46a8250cc1763d3/CLAUDE.md
repo: walterlow/freecut
kind: claude-md
stars: 1430
last_pushed: 2026-06-15T00:17:44Z
license: mit
score: 9
domains: [web-frontend, media-processing]
tags: [architecture-heavy, state-management, rules-driven]
curated: 2026-06-15
curated_by: config-scout
---

# walterlow/freecut — claude-md

**Why it's worth keeping:** It provides 'Implementation Rules' (e.g., mandatory action wrappers for store mutations) rather than just passive descriptions. The directory structure explicitly assigns functional responsibilities to folders, providing clear mental models for where logic belongs.

**Summary:** A comprehensive architectural blueprint for a complex video editor that defines strict rules for state management, mutations, and data structures.

**Source credibility:** Highly credible; a popular open-source project with significant stars and recent maintenance.

**Recency:** Extremely current, utilizing cutting-edge technologies like React 19 and Tailwind CSS 4.

**Source:** [walterlow/freecut/CLAUDE.md](https://github.com/walterlow/freecut/blob/fe595df738ffaf07713dd825b46a8250cc1763d3/CLAUDE.md) · 1430★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FreeCut Web

## Commands

```bash
npm run dev          # Vite dev server on port 5173
npm run build        # Production build
npm run lint         # Oxlint
npm run format       # Oxfmt
npm run format:check # Check formatting with Oxfmt
npm run test         # Vitest (watch mode)
npm run test:run     # Vitest (single run)
npm run routes       # Regenerate TanStack Router tree (tsr generate)
```

## Architecture

Browser-based multi-track video editor. React 19 + TypeScript + Vite.

```text
src/
├── features/              # User-facing UI modules
│   ├── editor/            # Editor shell, toolbar, panels, stores
│   ├── timeline/          # Multi-track timeline, actions, services
│   ├── preview/           # Preview canvas, transform gizmo, scrub renderer
│   ├── export/            # WebCodecs export pipeline (Web Worker)
│   ├── effects/           # GPU effect UI panels and registry
│   ├── keyframes/         # Keyframe animation, Bezier editor, easing
│   ├── media-library/     # Media import, metadata, OPFS proxies, transcription
│   ├── project-bundle/    # Project ZIP export/import
│   ├── projects/          # Project management
│   ├── scene-browser/     # Caption and scene se
```

</details>
