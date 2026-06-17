---
name: epam__ai-dial-core
source: https://github.com/epam/ai-dial-core/blob/118f7b8a6154a277f49373634226748bee0547d6/CLAUDE.md
repo: epam/ai-dial-core
kind: claude-md
stars: 659
last_pushed: 2026-06-15T07:38:53Z
license: apache-2.0
score: 9
domains: [backend-api, java]
tags: [gradle, api-gateway, microservices]
curated: 2026-06-15
curated_by: config-scout
---

# epam/ai-dial-core — claude-md

**Why it's worth keeping:** The mapping of modules to responsibilities and sub-packages provides the LLM with a high-level mental model, while specific Gradle command examples enable precise verification of changes.

**Summary:** Provides highly detailed build instructions including granular test execution patterns and a clear architectural hierarchy of modules and packages. It also clearly distinguishes between static and hot-reloadable dynamic configurations.

**Source credibility:** High; EPAM is a major enterprise software firm and the repository shows active maintenance.

**Recency:** Very current; utilizes modern stack (Java 21, Vert.x 4.5) and follows contemporary development patterns.

**Source:** [epam/ai-dial-core/CLAUDE.md](https://github.com/epam/ai-dial-core/blob/118f7b8a6154a277f49373634226748bee0547d6/CLAUDE.md) · 659★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Run

GitHub credentials are required for the private JClouds Maven package (hosted on GitHub Packages):

```bash
# Set credentials via environment variables
export GPR_USERNAME=<github_user>
export GPR_PASSWORD=<github_token>

# Build (skip tests)
./gradlew build -x test

# Run all tests
./gradlew test

# Run tests for a specific module
./gradlew :server:test

# Run a single test class
./gradlew :server:test --tests "com.epam.aidial.core.server.ResourceApiTest"

# Run a single test method
./gradlew :server:test --tests "com.epam.aidial.core.server.ResourceApiTest.testWorkflow"

# Checkstyle
./gradlew checkstyleMain checkstyleTest

# Run locally
./gradlew :server:run
```

At runtime, set `AIDIAL_SETTINGS` env var pointing to a JSON settings file (see `sample/aidial.settings.json`).

## Architecture

AI DIAL Core is an **HTTP reverse proxy / API gateway** for LLMs built on **Java 21** + **Eclipse Vert.x** (reactive, non-blocking). It exposes an OpenAI-compatible API and routes requests to backend AI providers (Azure OpenAI, AWS, GCP, etc.).

### Gradle Modul
```

</details>
