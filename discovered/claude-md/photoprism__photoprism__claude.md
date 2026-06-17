---
name: photoprism__photoprism__claude
source: https://github.com/photoprism/photoprism/blob/9605d87731fa14f48bfaa81526c023d3e2bb1783/.claude/CLAUDE.md
repo: photoprism/photoprism
kind: claude-md
stars: 39807
last_pushed: 2026-06-14T16:39:14Z
license: other
score: 9
domains: [backend-api, web-frontend, go-development]
tags: [comprehensive, architecture-mapping, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# photoprism/photoprism — claude-md

**Why it's worth keeping:** The directory-to-purpose mapping table is excellent for providing context without manual exploration, and providing exact `go test -run` patterns prevents slow full-suite executions.

**Summary:** This file provides highly granular build, test, and migration instructions alongside a structured architectural map of the codebase. It bridges the gap between high-level structure and specific CLI commands needed for development.

**Source credibility:** High; Photoprism is a mature, highly-starred open-source project with active development.

**Recency:** Current; it includes modern tools like Vitest and Vue 3.

**Source:** [photoprism/photoprism/.claude/CLAUDE.md](https://github.com/photoprism/photoprism/blob/9605d87731fa14f48bfaa81526c023d3e2bb1783/.claude/CLAUDE.md) · 39807★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository. Detailed rules are in `.claude/rules/*.md` files organized by topic.

## Build Commands

Run `make help` to list all available targets. Key commands:

**Backend (Go):**
- `make build-go` — build the `photoprism` binary (develop mode)
- `make build-all` — build backend + frontend
- `go build ./...` — compile all Go packages

**Frontend (Vue 3):**
- `make build-js` — production build of the frontend
- `make watch-js` — watch mode for frontend development (Ctrl+C to stop)

**Dependencies:**
- `make dep` — install all dependencies (TensorFlow models, ONNX models, JS packages)
- `make dep-js` — install JS dependencies only (`npm ci`). The `photoprism/develop` image and the repo `Makefile` both set `NPM_CONFIG_IGNORE_SCRIPTS=true`, so install scripts are skipped automatically; when running npm directly in an env without that default, pass `--ignore-scripts`. Rebuild native addons with `npm rebuild --ignore-scripts=false <pkg>` — a bare `npm rebuild` no-ops wherever the env default is active.

**Docker dev environment:**
- `make docker-build` — build local Docker image
- `do
```

</details>
