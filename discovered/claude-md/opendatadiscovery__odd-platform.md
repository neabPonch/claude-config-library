---
name: opendatadiscovery__odd-platform
source: https://github.com/opendatadiscovery/odd-platform/blob/19618ea29a6fcbbb5305d85253ab64a4a2f1bff7/CLAUDE.md
repo: opendatadiscovery/odd-platform
kind: claude-md
stars: 1408
last_pushed: 2026-06-15T23:22:11Z
license: apache-2.0
score: 9
domains: [full-stack, backend-java, web-frontend, devops]
tags: [multi-module, workflow-driven, architecture-heavy]
curated: 2026-06-16
curated_by: config-scout
---

# opendatadiscovery/odd-platform — claude-md

**Why it's worth keeping:** The 'Common Development Workflows' section provides exact sequences of actions (e.g., OpenAPI -> Code Gen -> Implementation) essential for agentic task execution. It also clearly differentiates between various state management tools to prevent pattern drift.

**Summary:** Provides highly detailed technical context, architectural patterns, and specific multi-step development workflows for a full-stack Java/React project.

**Source credibility:** Highly credible: a popular open-source data platform with significant stars and recent activity.

**Recency:** Very current; reflects modern development patterns like reactive Spring, Vite, and TanStack Query.

**Source:** [opendatadiscovery/odd-platform/CLAUDE.md](https://github.com/opendatadiscovery/odd-platform/blob/19618ea29a6fcbbb5305d85253ab64a4a2f1bff7/CLAUDE.md) · 1408★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ODD Platform is a data discovery and observability platform built with a Spring Boot backend (Java 17) and React/TypeScript frontend. The platform ingests, structures, and indexes metadata from data sources, providing REST APIs and a modern UI for data cataloging, lineage, quality monitoring, and collaboration.

## Repository Structure

The repository is a multi-module Gradle project:

- **odd-platform-api-contract**: OpenAPI spec code generation (generates Spring reactive interfaces from `odd-platform-specification/openapi.yaml`)
- **odd-platform-api**: Spring Boot backend (reactive WebFlux, R2DBC, JOOQ)
- **odd-platform-ui**: React/TypeScript frontend (Vite, Redux Toolkit, Material-UI)
- **odd-platform-specification**: OpenAPI specification files
- **tests**: Playwright end-to-end tests
- **docker**: Docker compose configurations for local development and demos

## Development Commands

### Backend (Java/Gradle)

Build the entire project:
```bash
./gradlew build
```

Build backend only (without UI):
```bash
./gradlew odd-platform-api:build -Pbu
```

</details>
