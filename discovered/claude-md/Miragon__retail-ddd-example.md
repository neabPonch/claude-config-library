---
name: Miragon__retail-ddd-example
source: https://github.com/Miragon/retail-ddd-example/blob/6354a933cf5beeeabf99520a450c4ae4220370ee/CLAUDE.md
repo: Miragon/retail-ddd-example
kind: claude-md
stars: 3
last_pushed: 2026-06-15T07:53:38Z
license: unknown
score: 9
domains: [backend-api, architecture, devops, kotlin]
tags: [ddd, hexagonal-architecture, gradle, spring-boot, multi-module]
curated: 2026-06-15
curated_by: config-scout
---

# Miragon/retail-ddd-example — claude-md

**Why it's worth keeping:** The inclusion of an explicit directory structure for the Hexagonal architecture pattern gives Claude clear instructions on where to place new code. It also provides specific orchestration commands for local development (Minikube/Helm) which is vital for agentic troubleshooting.

**Summary:** Provides exhaustive command templates for a complex multi-module Gradle/Spring Boot project and detailed architectural layering rules.

**Source credibility:** Small example project, but highly structured and professional documentation.

**Recency:** Very current; references React 19 and Spring Boot 3.5.3.

**Source:** [Miragon/retail-ddd-example/CLAUDE.md](https://github.com/Miragon/retail-ddd-example/blob/6354a933cf5beeeabf99520a450c4ae4220370ee/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build System & Development

This is a multi-module Gradle project using Kotlin and Spring Boot. Java 21 is required.

### Common Commands

**Build entire project:**

```bash
./gradlew build
```

**Run tests:**

```bash
./gradlew test
```

**Run specific service locally:**

```bash
./gradlew :services:shop:shop-backend:bootRun
./gradlew :services:delivery:delivery-backend:bootRun
./gradlew :services:warehouse:warehouse-backend:bootRun
./gradlew :services:shop:shop-mcp-client:bootRun
```

**Run single test:**

```bash
./gradlew :services:shop:shop-backend:test --tests "LoadArticlesServiceTest"
```

**Build Docker images:**

```bash
docker build -t shop-backend:local -f services/shop/shop-backend/Dockerfile .
```

### Frontend Development

The shop frontend is a React + Vite application:

**Frontend commands (in services/shop/shop-frontend/):**

```bash
npm run dev          # Start development server
npm run build        # Build for production  
npm run test:eslint  # Run ESLint
npm run apiGeneration # Generate API client from OpenAPI spec
```

**E2E Testing (in serv
```

</details>
