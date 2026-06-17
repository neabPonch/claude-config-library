---
name: seaworld008__chronodesk
source: https://github.com/seaworld008/chronodesk/blob/9ea92bab0d2e379c642a95de089f3c7e37def4c8/CLAUDE.md
repo: seaworld008/chronodesk
kind: claude-md
stars: 1
last_pushed: 2026-02-27T13:33:57Z
license: unknown
score: 7
domains: [backend-api, web-frontend, fullstack]
tags: [go, react, docker, make]
curated: 2026-06-16
curated_by: config-scout
---

# seaworld008/chronodesk — claude-md

**Why it's worth keeping:** The separation of commands by subdirectory (server/ vs web/) and the detailed explanation of internal folder patterns are highly effective for orienting an agent in nested repositories.

**Summary:** Provides a comprehensive structural map of a full-stack Go and React project, specifically emphasizing directory hierarchies and granular command execution.

**Source credibility:** A low-star personal project that demonstrates high-quality, professional documentation standards.

**Recency:** Current; uses modern technologies like Go 1.21, React 18, and Vite.

**Source:** [seaworld008/chronodesk/CLAUDE.md](https://github.com/seaworld008/chronodesk/blob/9ea92bab0d2e379c642a95de089f3c7e37def4c8/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a modern ticketing system built with Go (Gin) backend and React (TypeScript) frontend. The system supports multi-role permission control and real-time collaboration.

## Architecture

- **Backend**: Go 1.21+ with Gin framework, PostgreSQL database, Redis cache, JWT + OTP authentication
- **Frontend**: React 18+ with TypeScript, Vite build tool, shadcn/ui + TailwindCSS, TanStack Query for state management
- **Database**: PostgreSQL 15+ with GORM for ORM, Redis 7+ for caching
- **Deployment**: Docker & Docker Compose for containerization

## Development Commands

### Quick Start
```bash
# Start full development environment with Docker
make dev
# or
docker-compose up -d
```

### Backend (server/)
```bash
# Install dependencies
cd server && go mod tidy

# Run server in development mode
cd server && make run
# or with auto-migration enabled
cd server && make run-migrate

# Run database migrations
cd server && make migrate-all

# Run tests
cd server && make test
# or
cd server && go test ./...

# Build server
cd server && make build

# Format a
```

</details>
