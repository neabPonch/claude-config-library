---
name: joe714__pixelgw
source: https://github.com/joe714/pixelgw/blob/3890e79f42a08f7db41c61ba97b09b1039469346/CLAUDE.md
repo: joe714/pixelgw
kind: claude-md
stars: 26
last_pushed: 2026-01-02T04:06:05Z
license: apache-2.0
score: 9
domains: [backend-api, web-frontend, fullstack]
tags: [openapi, codegen, go, react]
curated: 2026-06-14
curated_by: config-scout
---

# joe714/pixelgw — claude-md

**Why it's worth keeping:** The explicit documentation of the 'Change Spec -> Regenerate Backend -> Regenerate Frontend' pipeline and warnings against manual edits of generated files are perfect for agentic workflows.

**Summary:** Provides a high-density guide for a Go/React project with a heavy emphasis on an OpenAPI-driven code generation workflow.

**Source credibility:** Small niche project with reasonable maintenance activity.

**Recency:** Highly relevant for current agent-based development patterns.

**Source:** [joe714/pixelgw/CLAUDE.md](https://github.com/joe714/pixelgw/blob/3890e79f42a08f7db41c61ba97b09b1039469346/CLAUDE.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
PixelGW is a self-hosted WebSocket gateway for managing Pixlet apps and serving them to low-resolution pixel displays. It provides a REST API backend (Go) and React frontend for managing channels, devices, and applets.

## Development Commands

### Building and Deployment
```bash
# Generate API bindings from OpenAPI spec (required after modifying pixelgw.yaml)
make generate

# Build Docker image with frontend assets
make build

# Deploy development environment (port 8081, with HMR)
make deploy_test

# Deploy production environment (port 8080)
make deploy_prod
```

### Frontend Development
```bash
# Navigate to web directory first
cd web

# Install dependencies
npm install

# Generate TypeScript API client from OpenAPI spec
npm run codegen

# Run development server with HMR
npm run dev

# Build production bundle
npm run build

# Run linter
npm run lint

# **Note:** Typically the staging server with HMR is running on
# http://localhost:8081/ at all times. Attempt to use it for testing
# changes, and if not running or it needs to be rebuilt, rebuild
```

</details>
