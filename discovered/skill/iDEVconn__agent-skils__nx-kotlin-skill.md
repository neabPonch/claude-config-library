---
name: iDEVconn__agent-skils__nx-kotlin-skill
source: https://github.com/iDEVconn/agent-skils/blob/7b88ec93f11f335e85c3f1a0da7a8163260c5b0f/NX_KOTLIN_SKILL.md
repo: iDEVconn/agent-skils
kind: skill
stars: 0
last_pushed: 2026-05-25T20:16:05Z
license: apache-2.0
score: 9
domains: [monorepo-management, jvm, kotlin, nx-workspace]
tags: [nx, kotlin, gradle, integration, polyglot]
curated: 2026-06-16
curated_by: config-scout
---

# iDEVconn/agent-skils — skill

**Why it's worth keeping:** Identifies high-friction 'gotchas' like disabling the configuration cache to allow specific task registration and provides exact, working file structures for polyglot environments.

**Summary:** Provides a specific, opinionated blueprint for integrating Kotlin/JVM subprojects into an Nx monorepo using @jnxplus/nx-gradle. It solves the architectural conflict between Gradle's root expectations and Nx's workspace structure.

**Source credibility:** High technical depth suggests a real-world developer's manual rather than generic documentation.

**Recency:** Very current, referencing recent Gradle/Kotlin versions and up-to-date plugin requirements.

**Source:** [iDEVconn/agent-skils/NX_KOTLIN_SKILL.md](https://github.com/iDEVconn/agent-skils/blob/7b88ec93f11f335e85c3f1a0da7a8163260c5b0f/NX_KOTLIN_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nx-kotlin-integration
description: Scaffold or maintain a Kotlin/JVM (Gradle Kotlin DSL) subproject inside a TypeScript-first Nx monorepo. Use whenever the user mentions Kotlin in Nx, Java in Nx, Gradle in Nx, @nx/gradle, @jnxplus/nx-gradle, adding a JVM app or ML service to an Nx workspace, "ml service in nx", "kotlin subproject", "scaffold kotlin app", troubleshooting `projectDependencyTask` not found, Gradle configuration cache errors in Nx, or WebStorm refusing to load the Kotlin plugin (`com.intellij.modules.java-capable`). Encodes the exact plugin choice, Gradle plugin versions, files to create, and gotchas discovered when integrating a Kotlin/JVM app under apps/ alongside existing React + NestJS workspaces.
---

# Nx + Kotlin/JVM (Gradle Kotlin DSL) Integration

This skill is a playbook for the specific job of dropping a Kotlin/JVM Gradle subproject into an Nx workspace that already has JS/TS apps. The advice is opinionated because the obvious-looking choices (the official `@nx/gradle` plugin, defaults from `gradle init`, leaving the configuration cache on) silently don't work in this layout. The notes below capture what does work and **why** — so when the next var
```

</details>
