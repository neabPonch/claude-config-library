---
name: JetBrains__kotlinconf-app
source: https://github.com/JetBrains/kotlinconf-app/blob/4937d1f4e5509214a606a73765d0a79ad9309bc0/CLAUDE.md
repo: JetBrains/kotlinconf-app
kind: claude-md
stars: 3524
last_pushed: 2026-06-05T12:11:26Z
license: apache-2.0
score: 9
domains: [kotlin-multiplatform, mobile, backend]
tags: [kmp, compose, ktor, gradle]
curated: 2026-06-17
curated_by: config-scout
---

# JetBrains/kotlinconf-app — claude-md

**Why it's worth keeping:** Explicitly details the complex custom source set hierarchy and dependency injection logic; provides exact build commands for multiple platform targets.

**Summary:** A high-density guide for a Kotlin Multiplatform project covering client-side DI, navigation, and KMP source sets alongside backend architecture.

**Source credibility:** Highly credible; official JetBrains repository with high star count and active maintenance.

**Recency:** 

**Source:** [JetBrains/kotlinconf-app/CLAUDE.md](https://github.com/JetBrains/kotlinconf-app/blob/4937d1f4e5509214a606a73765d0a79ad9309bc0/CLAUDE.md) · 3524★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

The official KotlinConf app — a Kotlin Multiplatform project serving Android, iOS, JVM desktop, and WebAssembly clients, backed by a Ktor server. All client UI is shared via Compose Multiplatform.

## Build & Run Commands

```bash
# Run desktop app (hot reload enabled)
./gradlew :app:desktopApp:hotRun -DmainClass=org.jetbrains.kotlinconf.MainKt

# Run web app (wasmJs target, development mode)
./gradlew :app:webApp:wasmJsBrowserDevelopmentRun

# Run backend server
./gradlew :backend:run

# Run backend tests
./gradlew :backend:test

# Run shared module tests (JVM target)
./gradlew :app:shared:jvmTest

# Run core module tests
./gradlew :core:jvmTest

# Bump version across all platforms + generate library definitions
./gradlew prepareRelease
```

Android uses the `app.androidApp` run configuration in IDE; iOS uses `KotlinConfAppScheme`.

## Module Structure

```
:core                 — Shared data models (Conference, Session, Speaker, VoteInfo, Score, AppConfig, etc.)
                        Used by both client and backend. No UI, no platform code.

:app
```

</details>
