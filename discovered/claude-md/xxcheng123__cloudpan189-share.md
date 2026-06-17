---
name: xxcheng123__cloudpan189-share
source: https://github.com/xxcheng123/cloudpan189-share/blob/25bc79f47080b551cb69b862db3f0d35ede71acb/CLAUDE.md
repo: xxcheng123/cloudpan189-share
kind: claude-md
stars: 193
last_pushed: 2025-10-14T03:15:06Z
license: mit
score: 8
domains: [backend-api, web-frontend, go, vue]
tags: [architecture-mapping, multi-stack, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# xxcheng123/cloudpan189-share — claude-md

**Why it's worth keeping:** Excellent use of structured service mapping to explain business logic hierarchy and explicit CLI command sections for cross-stack development.

**Summary:** Provides a high-density technical manual covering build workflows, dual-stack architecture (Go/Vue), and strict communication constraints.

**Source credibility:** High; based on a popular open-source tool with 193 stars.

**Recency:** Recent enough (8 months) to be highly relevant to current Go/Vue ecosystems.

**Source:** [xxcheng123/cloudpan189-share/CLAUDE.md](https://github.com/xxcheng123/cloudpan189-share/blob/25bc79f47080b551cb69b862db3f0d35ede71acb/CLAUDE.md) · 193★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Memory Requirements

**IMPORTANT**: All communication and responses must be in Chinese (中文). Claude must use Chinese for all interactions with the user, including:
- 所有回复必须使用中文
- 代码注释和文档说明使用中文
- 错误信息和提示使用中文
- 任何交流都必须用中文进行

## Common Development Commands

### Building the Project
- `make build` - Build both frontend and backend
- `make build-frontend` - Build frontend only (Vue.js)
- `make build-backend` - Build backend only (Go binary)
- `make build-multi-arch` - Build for multiple architectures (Linux, Windows, macOS)

### Development
- `make dev` - Start development server (backend only)
- `go run ./cmd/main.go` - Direct backend development
- Frontend development: `cd fe && npm run dev` (starts Vite dev server on port 5173)

### Testing and Quality
- `make test` - Run Go tests
- `make lint` - Run golangci-lint
- Frontend linting: `cd fe && npm run lint` (ESLint + stylelint)
- Frontend formatting: `cd fe && npm run format` (Prettier)

### Docker
- `make docker-build` - Build Docker image
- `make docker-run` - Run Docker container
- `make docker-stop` - Stop Docke
```

</details>
