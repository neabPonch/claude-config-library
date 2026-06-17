---
name: exacaster__lighter
source: https://github.com/exacaster/lighter/blob/86c215be5746c8f966eef4a8e33d8c2dac29a40d/CLAUDE.md
repo: exacaster/lighter
kind: claude-md
stars: 112
last_pushed: 2026-03-11T18:04:17Z
license: mit
score: 9
domains: [backend-api, web-frontend, devops]
tags: [full-stack, java, react, architectural-map]
curated: 2026-06-15
curated_by: config-scout
---

# exacaster/lighter — claude-md

**Why it's worth keeping:** It provides specific command examples (like running single tests) and maps business domains directly to file paths, which is critical for large repos.

**Summary:** A high-density guide providing actionable build commands and a detailed structural map of the project's domain logic.

**Source credibility:** Solid open-source project with active maintenance.

**Recency:** Very current, utilizing modern tech stacks like React 19 and Micronaut 4.

**Source:** [exacaster/lighter/CLAUDE.md](https://github.com/exacaster/lighter/blob/86c215be5746c8f966eef4a8e33d8c2dac29a40d/CLAUDE.md) · 112★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is Lighter

Lighter is an open-source web UI and REST API for running Apache Spark batch jobs and interactive sessions on Kubernetes or Apache Hadoop YARN (inspired by Apache Livy).

## Commands

### Backend (server/)

```bash
cd server
./gradlew build              # Build JAR and run tests
./gradlew build -x test      # Build without tests
./gradlew test               # Run tests only
./gradlew test --tests "com.exacaster.lighter.SomeTest"  # Run single test
./gradlew build -PSPARK_VERSION=3.5.8  # Build with specific Spark version
```

### Frontend (frontend/)

```bash
cd frontend
yarn install    # Install dependencies
yarn start      # Dev server on port 3000 (proxies /lighter/api to localhost:8080)
yarn build      # Production build → dist/
yarn lint       # ESLint
yarn format     # Prettier
```

### Docker

```bash
docker build -t lighter .    # Multi-stage build from project root
cd dev && docker-compose up  # Local dev environment
```

## Architecture

### Backend (Java 17 / Micronaut 4)

Entry point: `server/src/main/java/com/exacaster/lighter/Applica
```

</details>
