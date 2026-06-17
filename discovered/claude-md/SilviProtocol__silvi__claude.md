---
name: SilviProtocol__silvi__claude
source: https://github.com/SilviProtocol/silvi/blob/305a5e8b614e4ad5bc9ee6bb9d05cec2c88bfe97/.claude/claude.md
repo: SilviProtocol/silvi
kind: claude-md
stars: 4
last_pushed: 2026-04-18T10:02:58Z
license: mit
score: 9
domains: [web-frontend, backend-api, geospatial]
tags: [environment-status, service-orchestration, technical-debt]
curated: 2026-06-15
curated_by: config-scout
---

# SilviProtocol/silvi — claude-md

**Why it's worth keeping:** The use of status tables for running services, explicit warnings about port conflicts (Port 5002), and documented known issues allows an AI to debug environment errors immediately.

**Summary:** A high-density documentation file that provides a comprehensive ground truth for local vs. production environments and multi-service architectures.

**Source credibility:** High; active repository with specific, up-to-date technical details.

**Recency:** Very current, referencing modern versions like Next.js 15 and PostgreSQL 17.

**Source:** [SilviProtocol/silvi/.claude/claude.md](https://github.com/SilviProtocol/silvi/blob/305a5e8b614e4ad5bc9ee6bb9d05cec2c88bfe97/.claude/claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Treekipedia & Ontology-Generator Documentation
**Last Updated**: January 5, 2026
**Version**: Production + Local Development Environment

> **FOR ONBOARDING**: Read [GO.md](.claude/project-management/GO.md) first for complete project context and onboarding procedure.
>
> **DOCUMENTATION SYSTEM** (in `.claude/project-management/`):
> - [GO.md](.claude/project-management/GO.md) - Onboarding workflow (start here)
> - [ACTIVE.md](.claude/project-management/ACTIVE.md) - Current production status and metrics
> - [TODO.md](.claude/project-management/TODO.md) - Development roadmap and priorities
> - [CHANGELOG.md](.claude/project-management/CHANGELOG.md) - History of completed work
> - This file (CLAUDE.md) - Development guide and patterns

This repository contains two interconnected systems: **Treekipedia** (web platform for tree species knowledge) and **Ontology-Generator** (semantic knowledge graph builder).

---

## Current Environment Status

| Service | Status | Location | Details |
|---------|--------|----------|---------|
| **Local Frontend** | ✅ Running | http://localhost:3001 | Next.js 15 dev server |
| **Local Backend** | ✅ Running | http://localhost:5001 | PostgreSQL 17 + Pos
```

</details>
