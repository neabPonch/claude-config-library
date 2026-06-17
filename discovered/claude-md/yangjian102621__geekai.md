---
name: yangjian102621__geekai
source: https://github.com/yangjian102621/geekai/blob/64832a2a04945d3c4d51582730a637d5d5d26325/CLAUDE.md
repo: yangjian102621/geekai
kind: claude-md
stars: 4660
last_pushed: 2026-05-24T02:14:40Z
license: apache-2.0
score: 7
domains: [fullstack, backend-api, web-frontend]
tags: [go, vue3, architecture, build-commands]
curated: 2026-06-15
curated_by: config-scout
---

# yangjian102621/geekai — claude-md

**Why it's worth keeping:** Excellent separation of backend vs frontend build processes and high-level mapping of the business logic layer (handler/service/store).

**Summary:** Provides a comprehensive breakdown of a full-stack Go/Vue architecture including build commands, directory responsibilities, and API routing.

**Source credibility:** High; 4600+ stars and recent activity indicate a popular, well-maintained repository.

**Recency:** Current; uses modern tech stacks like Vue 3/Vite/Pinia which aligns with current development standards.

**Source:** [yangjian102621/geekai/CLAUDE.md](https://github.com/yangjian102621/geekai/blob/64832a2a04945d3c4d51582730a637d5d5d26325/CLAUDE.md) · 4660★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

### Go Backend (api/)
- **Development**: `cd api && go run main.go` (uses config.toml)
- **Build**: `cd api && make` (builds both amd64 and arm64 binaries)
- **Individual builds**: `make amd64` or `make arm64`
- **Clean**: `make clean`
- **Config**: Copy `config.sample.toml` to `config.toml` and configure

### Web Frontend (web/)
- **Development**: `cd web && npm run dev` (runs on Vite dev server with --host)
- **Build**: `cd web && npm run build`
- **Lint**: `cd web && npm run lint` (ESLint with auto-fix)

### Testing
- Backend tests: `cd api/test && bash run_crawler_test.sh`
- No specific frontend test configuration found

## Project Architecture

### Backend (Go)
- **Framework**: Gin web framework with dependency injection via uber-go/fx
- **Database**: GORM with MySQL, Redis for caching, LevelDB for local storage
- **Authentication**: JWT tokens with Redis session storage
- **Middleware**: CORS, authorization, parameter handling, static resource serving
- **Structure**:
  - `handler/`: HTTP request handlers (REST API endpoints)
  - `service/`:
```

</details>
