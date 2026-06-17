---
name: grantstephens__gather
source: https://github.com/grantstephens/gather/blob/d21cb95a5e427c26629b87a7323abc405379df67/CLAUDE.md
repo: grantstephens/gather
kind: claude-md
stars: 4
last_pushed: 2026-06-14T10:58:24Z
license: other
score: 9
domains: [fullstack, web-app, backend-api]
tags: [makefiles, architecture, business-logic, go, preact]
curated: 2026-06-15
curated_by: config-scout
---

# grantstephens/gather — claude-md

**Why it's worth keeping:** It explicitly documents business logic/access control rules and environmental patterns (like DEV mode proxying), which prevents the AI from making invalid architectural assumptions.

**Summary:** Provides comprehensive full-stack context including specific build workflows, directory mappings, and data model constraints.

**Source credibility:** High-quality personal project with active maintenance and clear documentation structure.

**Recency:** Highly current, utilizing modern tools like Vite and PocketBase.

**Source:** [grantstephens/gather/CLAUDE.md](https://github.com/grantstephens/gather/blob/d21cb95a5e427c26629b87a7323abc405379df67/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Gather is a community calendar application built with Go (PocketBase backend) and Preact (frontend). It supports event submission, moderation workflows, ActivityPub federation, RSS/iCal feeds, and location-based events using OSM data.

## Development Commands

### Quick Start
```bash
make dev          # Build backend, start Vite + proxied backend, auto-seed data
```

### Backend Development
```bash
make build-backend   # Build Go binary (includes embedded frontend)
make dev-backend     # Run backend in dev mode (proxies to Vite at :5173)
make run             # Start server (assumes already built)
```

### Frontend Development
```bash
cd frontend && npm run dev     # Or: make dev-frontend
cd frontend && npm run build   # Or: make build-frontend
```

### Data Management
```bash
make setup-admin   # Create admin user (idempotent)
make seed          # Seed dummy data (requires running server)
make reset         # Clean everything including database
```

### Production
```bash
make prod          # Build, setup admin, seed, and start server
```

**Dev
```

</details>
