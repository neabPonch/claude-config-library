---
name: paulmanoni__nexus
source: https://github.com/paulmanoni/nexus/blob/7574498654da467e4339ae275067e81c379e7061/CLAUDE.md
repo: paulmanoni/nexus
kind: claude-md
stars: 3
last_pushed: 2026-06-15T11:22:57Z
license: mit
score: 9
domains: [backend-api, web-frontend, go-framework]
tags: [viteless, fullstack-go, embedded-spa, config-driven]
curated: 2026-06-15
curated_by: config-scout
---

# paulmanoni/nexus — claude-md

**Why it's worth keeping:** It provides high-signal architectural patterns like how HMR proxying works between ports and how TOML configurations map to both Go and Frontend environments.

**Summary:** This file acts as a comprehensive technical manual for the 'nexus' framework, explaining its unique zero-Node frontend model and backend integration.

**Source credibility:** High; the project is actively maintained and provides a very specific, specialized developer experience.

**Recency:** 

**Source:** [paulmanoni/nexus/CLAUDE.md](https://github.com/paulmanoni/nexus/blob/7574498654da467e4339ae275067e81c379e7061/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# nexus — framework guide for Claude Code

nexus is a Go backend framework: typed reflective handlers over REST + GraphQL +
WebSocket, fx-based dependency injection, an embedded **viteless** frontend (a
zero-Node "Vite for Go"), and a live introspection dashboard at `/__nexus`. This file
tells you how to use every feature. Verify APIs against the installed version; `nexus
docs <topic>` prints an inline quick-reference for any feature (`nexus docs --list`).

Import path: `github.com/paulmanoni/nexus`. Pure-Go build — no CGO, no build tags.
**No Node/npm is required** for the frontend, at dev, build, or run time; the runtime
is a single Go binary with the SPA embedded.

---

## 1. Frontend (viteless, embedded SPA)

nexus serves a Vue/React/TS SPA via the embedded **viteless** engine
(`github.com/paulmanoni/viteless`) — a zero-Node implementation of the Vite dev/build
model in Go (esbuild + a WASM QuickJS engine). `nexus build` produces `web/dist` and
`go build` embeds it via `//go:embed`. No npm, no `node_modules`, no Node by default.

**Dependencies & fidelity (auto-detected, highest available wins):**
1. **Real Vite installed** (`web/node_modules/.bin/vite`) → viteless delegates to
```

</details>
