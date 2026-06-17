---
name: mi2odev__siara
source: https://github.com/mi2odev/siara/blob/51c5f2a858f3e0e9f0f15b8ed7917b2b4cfaff34/CLAUDE.md
repo: mi2odev/siara
kind: claude-md
stars: 1
last_pushed: 2026-06-14T16:06:55Z
license: unknown
score: 9
domains: [backend-api, machine-learning-ops, web-frontend]
tags: [monorepo, multi-runtime, architectural-context]
curated: 2026-06-14
curated_by: config-scout
---

# mi2odev/siara — claude-md

**Why it's worth keeping:** It includes critical 'don't touch' warnings regarding intentional typos and deep explanations of schema/middleware logic that prevent the AI from breaking the system during refactors.

**Summary:** A comprehensive architectural guide for a multi-runtime monorepo involving Node.js, Flask (ML), and React.

**Source credibility:** Low star count indicates a niche or private project, but the technical depth suggests a sophisticated real-world codebase.

**Recency:** Extremely current; explicitly mentions React 19 and Tailwind v4.

**Source:** [mi2odev/siara/CLAUDE.md](https://github.com/mi2odev/siara/blob/51c5f2a858f3e0e9f0f15b8ed7917b2b4cfaff34/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository layout

This is a multi-runtime monorepo with three cooperating processes — there is no top-level orchestration script, each must be started independently:

- `api/` — Node.js/Express backend (entry: [api/index.js](api/index.js)). Owns all HTTP routes under `/api/*`, JWT auth, PostgreSQL access, Socket.IO notifications, and proxies ML calls to the Flask service.
- `api/contollers/Model/ml_service.py` — Flask ML microservice on port `8000`. Loads joblib models for driver-quiz risk and danger-zone severity, plus SHAP explainers. The Node API talks to it via `ML_SERVICE_BASE_URL` (default `http://localhost:8000`).
- `client/` — React 19 + Vite frontend (default port `5173`).

Note: the controllers folder is intentionally spelled `contollers` (typo baked into all `require` paths — do not rename).

## Common commands

Backend (Node API, port `5000` by default):
```bash
cd api && npm start          # nodemon index.js
node scripts/diagnoseNotifications.js   # check notification listener/socket plumbing
node scripts/testReportValidator.js     # smoke-test ML re
```

</details>
