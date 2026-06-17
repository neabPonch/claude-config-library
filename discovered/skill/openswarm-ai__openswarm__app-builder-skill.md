---
name: openswarm-ai__openswarm__app-builder-skill
source: https://github.com/openswarm-ai/openswarm/blob/78fbbebccd1d50df4f8f00b3531ba682b2448bd3/backend/apps/outputs/app_builder_skill.md
repo: openswarm-ai/openswarm
kind: skill
stars: 711
last_pushed: 2026-06-16T02:00:40Z
license: mit
score: 9
domains: [web-frontend, agents-ai, software-architecture]
tags: [react, vite, mui, architectural-patterns, performance]
curated: 2026-06-16
curated_by: config-scout
---

# openswarm-ai/openswarm — skill

**Why it's worth keeping:** Provides critical performance optimization rules (preventing MUI barrel imports) and a decision tree for choosing project structures to minimize build times.

**Summary:** A highly prescriptive architectural guide that branches logic between lightweight single-file apps and full-stack React workspaces.

**Source credibility:** High; part of the OpenSwarm mission control project with active maintenance.

**Recency:** Very current, utilizing modern stacks like React 18, Vite, and TypeScript.

**Source:** [openswarm-ai/openswarm/backend/apps/outputs/app_builder_skill.md](https://github.com/openswarm-ai/openswarm/blob/78fbbebccd1d50df4f8f00b3531ba682b2448bd3/backend/apps/outputs/app_builder_skill.md) · 711★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# App Builder — Platform Reference

You are building an **App** inside OpenSwarm. The workspace you're working
in is a **React 18 + TypeScript + Vite** project (with an optional FastAPI
backend you can opt into on demand). It's served live to a webview, so it
behaves like a real browser tab — cross-origin `fetch`, popups, mic/camera,
clipboard, anything a normal web page does.

---

## STEP 0 — pick the right shape for the app

Before writing any code, decide whether this app should be **workspace**
(full React/MUI, the default) or **lightweight** (one self-contained
`index.html`). Picking wrong wastes the user's time: the workspace path
spends ~10-30 s pre-bundling MUI and React on first preview, which is
pointless when the app is a 200-line Three.js demo.

**Lightweight** when ALL apply:
- One page, no route navigation
- No persisted server state (no DB-shaped data the user comes back to)
- No real backend logic (just CDN libraries, in-memory state)
- The whole UI is essentially one of: canvas/WebGL scene, single-file
  visualization (D3/Plotly/Chart.js), single-purpose tool (formatter,
  calculator, color picker), tiny game or simulator

**Workspace** (this document's default) w
```

</details>
