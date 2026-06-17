---
name: AndriyKalashnykov__animal-rescue
source: https://github.com/AndriyKalashnykov/animal-rescue/blob/1d75f026852a3512ed6a37114ca9f3739f5d4d46/CLAUDE.md
repo: AndriyKalashnykov/animal-rescue
kind: claude-md
stars: 6
last_pushed: 2026-06-08T06:32:24Z
license: apache-2.0
score: 8
domains: [backend-api, web-frontend, devops]
tags: [spring-boot, multi-module, make, gradle]
curated: 2026-06-15
curated_by: config-scout
---

# AndriyKalashnykov/animal-rescue — claude-md

**Why it's worth keeping:** Provides explicit, ready-to-use terminal commands for building, testing, and running different modules, which is critical for agentic autonomy. The inclusion of specific test credentials (alice/test) and API endpoints adds high-value context for task execution.

**Summary:** A well-structured guide for a multi-module application consisting of a Spring Boot backend and Node.js frontend. It clearly maps out the repository structure and the lifecycle commands required to run the project.

**Source credibility:** A specialized sample repository with recent activity.

**Recency:** 

**Source:** [AndriyKalashnykov/animal-rescue/CLAUDE.md](https://github.com/AndriyKalashnykov/animal-rescue/blob/1d75f026852a3512ed6a37114ca9f3739f5d4d46/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Animal Rescue is a Java Spring Boot sample application demonstrating VMware's opinionated approach to building applications with Tanzu products. It features a reactive Spring WebFlux backend with R2DBC (H2), a Node.js frontend, and Cypress end-to-end tests.

**Owner:** AndriyKalashnykov/animal-rescue

## Tech Stack

- **Backend:** Java 11, Spring Boot 2.5.5, Spring WebFlux, Spring Security (OAuth2 Resource Server), R2DBC with H2
- **Frontend:** Node.js 14.x, served separately
- **E2E Tests:** Cypress
- **Build:** Gradle (multi-project: backend, frontend, e2e)
- **CI:** GitHub Actions (`.github/workflows/main.yml`, `.github/workflows/cleanup-runs.yml`)

## Repository Layout

```
backend/          Spring Boot WebFlux backend (Gradle subproject)
frontend/         Node.js frontend application (Gradle subproject)
e2e/              Cypress end-to-end tests (Gradle subproject)
scripts/          Helper scripts (local.sh for dev lifecycle)
docs/             Documentation images
gradle/           Gradle wrapper files
build.gradle      Root Gradle build
settings.gradle   Multi-project settings (backend, frontend, e2e)
Makefile           Dev commands (build, t
```

</details>
