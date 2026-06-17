---
name: Open-MBEE__flexo-mms-sysmlv2
source: https://github.com/Open-MBEE/flexo-mms-sysmlv2/blob/bf462e22b945e3065e96abef2d84237a78bbfc35/CLAUDE.md
repo: Open-MBEE/flexo-mms-sysmlv2
kind: claude-md
stars: 13
last_pushed: 2026-05-12T17:55:29Z
license: apache-2.0
score: 9
domains: [backend-api, kotlin, jvm]
tags: [kotlin, ktor, microservice, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Open-MBEE/flexo-mms-sysmlv2 — claude-md

**Why it's worth keeping:** The 'Common Patterns' section is exceptional; it explicitly instructs the AI on how to use specific extension functions for HTTP calls and routing logic, ensuring generated code follows project-specific idioms.

**Summary:** A comprehensive technical guide covering tech stack, directory mapping, build/test workflows, and architectural nuances.

**Source credibility:** High-quality open-source engineering from OpenMBEE with recent activity (1 month ago).

**Recency:** Highly current; utilizes modern toolchains including JVM 21 and Ktor 3.x.

**Source:** [Open-MBEE/flexo-mms-sysmlv2/CLAUDE.md](https://github.com/Open-MBEE/flexo-mms-sysmlv2/blob/bf462e22b945e3065e96abef2d84237a78bbfc35/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Flexo MMS SysML v2 Microservice — a REST/HTTP adapter that implements the [SysML v2 API and Services](https://github.com/Systems-Modeling/SysML-v2-API-Services) specification on top of the OpenMBEE Flexo Model Management System (MMS) Layer 1. It translates SysML v2 domain concepts (Projects, Commits, Elements, Branches, Tags, Queries) into RDF graph operations against a triplestore via the MMS Layer 1 service.

## Tech Stack

- **Language:** Kotlin (JVM toolchain 21)
- **Framework:** Ktor 3.x (Netty engine)
- **Serialization:** kotlinx.serialization (JSON, with `@type` class discriminator)
- **RDF/SPARQL:** Apache Jena 6.x (jena-arq, jena-querybuilder)
- **Build:** Gradle 8.10.2 (Kotlin DSL, `build.gradle.kts`)
- **Testing:** Kotest 6.x (StringSpec style) + JUnit 5 + Ktor test host
- **CI:** CircleCI (`.circleci/config.yml`)
- **Code Quality:** SonarCloud + JaCoCo
- **Container:** Docker (Eclipse Temurin 21, multi-stage build)

## Repository Layout

```
src/main/kotlin/org/openmbee/flexo/sysmlv2/
  AppMain.kt            # Ktor application module, routing setup, FlexoConfig
  Configuration.kt      # HSTS and Compression plugin config
  Flexo.kt
```

</details>
