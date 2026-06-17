---
name: kotest__kotest
source: https://github.com/kotest/kotest/blob/24a4dc4420d09856029e02cf6516d0a9d38f2188/CLAUDE.md
repo: kotest/kotest
kind: claude-md
stars: 4779
last_pushed: 2026-06-14T13:32:27Z
license: apache-2.0
score: 9
domains: [kotlin, testing-framework, multiplatform]
tags: [build-instructions, architecture-overview, coding-standards, kmp]
curated: 2026-06-15
curated_by: config-scout
---

# kotest/kotest — claude-md

**Why it's worth keeping:** The project structure tree and 'Common Tasks' sections turn an AI into a contributor by providing precise navigation and implementation patterns. It also explicitly notes critical environment constraints like JVM heap size.

**Summary:** Provides high-level architectural context, specific build commands for various targets, and a detailed module hierarchy.

**Source credibility:** High; Kotest is a widely-used, highly starred Kotlin library with active maintenance.

**Recency:** Current; covers modern KMP and Wasm targets.

**Source:** [kotest/kotest/CLAUDE.md](https://github.com/kotest/kotest/blob/24a4dc4420d09856029e02cf6516d0a9d38f2188/CLAUDE.md) · 4779★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Kotest - Working with this Codebase

## What is Kotest

Kotest is a Kotlin Multiplatform testing framework comprising three pillars: a test framework with 9+ spec styles, an assertion/matchers library, and a property-based testing engine. It targets JVM, JS, WasmJS, WasmWASI, and all major Native platforms (Linux, macOS, Windows, iOS, tvOS, watchOS).

## Build and Test

```bash
# Full check (all platforms enabled locally by default)
./gradlew check

# JVM-only check (much faster for most changes)
./gradlew check -PjvmOnly=true

# Single module
./gradlew :kotest-assertions:kotest-assertions-core:check
./gradlew :kotest-framework:kotest-framework-engine:jvmTest

# API compatibility check (required before PR)
./gradlew apiCheck

# Regenerate API dump after public API changes
./gradlew apiDump
```

Gradle properties `kotest_enableKotlinJs` and `kotest_enableKotlinNative` in `gradle.properties` control which targets are built. Set to `false` for faster local iteration when working on JVM-only code.

The project requires JVM heap of 8GB (`-Xmx8g` in `gradle.properties`). Gradle parallel execution and caching are enabled by default.

## Project Structure

```
kotest-common/
```

</details>
