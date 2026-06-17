---
name: tddworks__openai-kotlin
source: https://github.com/tddworks/openai-kotlin/blob/d02d678103d2ba9e254e4a09e9703c412ab22a12/CLAUDE.md
repo: tddworks/openai-kotlin
kind: claude-md
stars: 53
last_pushed: 2025-12-18T08:53:25Z
license: apache-2.0
score: 8
domains: [kotlin, multiplatform, api-client]
tags: [gradle, architecture, testing, kmp]
curated: 2026-06-16
curated_by: config-scout
---

# tddworks/openai-kotlin — claude-md

**Why it's worth keeping:** It bridges the gap between 'how to run' and 'how it works' by documenting key interfaces, design patterns (Provider/Gateway), and specific module responsibilities.

**Summary:** Combines platform-specific Gradle commands with a high-level architectural map of the multiplatform modules.

**Source credibility:** The repository has respectable social proof for a niche library and is reasonably well-maintained.

**Recency:** Highly relevant; the structure follows current Kotlin Multiplatform standards which Claude Code handles well.

**Source:** [tddworks/openai-kotlin/CLAUDE.md](https://github.com/tddworks/openai-kotlin/blob/d02d678103d2ba9e254e4a09e9703c412ab22a12/CLAUDE.md) · 53★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Development Commands

### Building the Project
```bash
./gradlew build                 # Build all modules
./gradlew clean build           # Clean and build all modules
./gradlew assemble             # Assemble outputs without running tests
```

### Running Tests
```bash
./gradlew test                  # Run tests for all platforms
./gradlew jvmTest              # Run JVM tests only
./gradlew macosArm64Test      # Run macOS ARM64 tests
./gradlew iosSimulatorArm64Test # Run iOS simulator tests
./gradlew allTests             # Run tests for all targets with aggregated report
./gradlew check                # Run all verification tasks
```

### Test Coverage
```bash
./gradlew koverHtmlReport      # Generate HTML coverage report for all code
./gradlew koverXmlReport       # Generate XML coverage report
./gradlew koverVerify          # Run coverage verification (min 86% required)
```

### Running Specific Module Tests
```bash
./gradlew :openai-client:openai-client-core:test
./gradlew :anthropic-client:anthropic-client-core:test
./gradlew :ollama-client:ollama-
```

</details>
