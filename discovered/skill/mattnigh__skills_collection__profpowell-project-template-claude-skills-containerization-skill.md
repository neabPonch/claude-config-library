---
name: mattnigh__skills_collection__profpowell-project-template-claude-skills-containerization-skill
source: https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/ProfPowell__project-template__claude__skills__containerization__SKILL.md
repo: mattnigh/skills_collection
kind: skill
stars: 23
last_pushed: 2025-12-31T03:21:29Z
license: unknown
score: 8
domains: [devops, backend, security]
tags: [docker, nodejs, containerization, production-ready]
curated: 2026-06-16
curated_by: config-scout
---

# mattnigh/skills_collection — skill

**Why it's worth keeping:** Includes essential production nuances like non-root user configuration, volume mounting exclusion for node_modules in dev, and specific health check commands.

**Summary:** Provides highly optimized, multi-stage Docker patterns for Node.js applications including production and development environments.

**Source credibility:** Reasonable; follows modern industry standards despite modest star count.

**Recency:** Current; utilizes Node 20 and modern Docker best practices.

**Source:** [mattnigh/skills_collection/collection/ProfPowell__project-template__claude__skills__containerization__SKILL.md](https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/ProfPowell__project-template__claude__skills__containerization__SKILL.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: containerization
description: Build and deploy Docker containers for Node.js applications. Use when containerizing applications, optimizing Docker builds, or configuring container security.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
---

# Containerization Skill

Build secure, optimized Docker containers for Node.js applications.

## Core Principles

| Principle | Description |
|-----------|-------------|
| Minimal Images | Use slim base images, multi-stage builds |
| Non-root User | Never run as root in production |
| Layer Caching | Order Dockerfile for optimal caching |
| Security First | No secrets in images, scan for vulnerabilities |
| Reproducible | Pin versions, use lock files |

## Project Structure

```
project/
├── Dockerfile              # Production image
├── Dockerfile.dev          # Development with hot reload
├── docker-compose.yml      # Multi-container orchestration
├── docker-compose.dev.yml  # Development overrides
├── .dockerignore           # Files to exclude from build
└── .env.example            # Environment variable template
```

## Production Dockerfile

### Node.js Application

```dockerfile
# syntax=docker/dockerfile:1

# Stage 1: Depe
```

</details>
