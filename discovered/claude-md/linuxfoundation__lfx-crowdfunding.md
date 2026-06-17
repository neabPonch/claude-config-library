---
name: linuxfoundation__lfx-crowdfunding
source: https://github.com/linuxfoundation/lfx-crowdfunding/blob/784a140dab396c5bb092800ea6392e7dde2df646/CLAUDE.md
repo: linuxfoundation/lfx-crowdfunding
kind: claude-md
stars: 1
last_pushed: 2026-06-16T06:09:51Z
license: mit
score: 9
domains: [backend-api, web-frontend, devops]
tags: [monorepo, go, nuxt, architecture-guidance, agentic-instructions]
curated: 2026-06-16
curated_by: config-scout
---

# linuxfoundation/lfx-crowdfunding — claude-md

**Why it's worth keeping:** It includes highly effective agent-specific instructions like skill-loading workflows (uikit) and strict file-location rules for TypeScript types.

**Summary:** A comprehensive monorepo guide that maps specific commands, architectural layers, and environment requirements for both Go and Nuxt/Vue.

**Source credibility:** High; part of a managed Linux Foundation repository.

**Recency:** Current; references modern technologies including Nuxt 4 and Node 22.

**Source:** [linuxfoundation/lfx-crowdfunding/CLAUDE.md](https://github.com/linuxfoundation/lfx-crowdfunding/blob/784a140dab396c5bb092800ea6392e7dde2df646/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Kubernetes-native rewrite of a legacy Lambda-based crowdfunding platform. It is a monorepo containing:

- `backend/` — Go HTTP API (Chi router, PostgreSQL, Stripe)
- `frontend/` — Nuxt 4 BFF (Vue 3, TypeScript, Tailwind, PrimeVue)

Both are independently deployed to the LFX v2 shared Kubernetes cluster via ArgoCD GitOps (`linuxfoundation/lfx-v2-argocd`).

## Backend Commands (Go)

All commands run from `backend/`:

```bash
make deps          # Download Go module dependencies
make build         # Compile binary → bin/initiatives-api
make run           # Build and run locally (requires .env)
make test          # Run unit tests with race detector
make fmt           # Format Go code (gofmt + goimports)
make lint          # Run golangci-lint
make license-check # Verify SPDX license headers on .go files
make db-seed       # Load dev seed data (localhost only)
make docker-build  # Build Docker image
make deploy-kind   # Deploy to local Kind cluster with Helm
```

Entry points:
- `cmd/initiatives-api/` — HTTP API server (port 8080, `GET /livez`
```

</details>
