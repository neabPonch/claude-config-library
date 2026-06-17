---
name: byteground__Ghostly
source: https://github.com/byteground/Ghostly/blob/2c33f06abd2709ce940a3385d026c8ea7e5cdb3d/CLAUDE.md
repo: byteground/Ghostly
kind: claude-md
stars: 14
last_pushed: 2026-02-08T14:31:50Z
license: mit
score: 9
domains: [mobile, kotlin-multiplatform]
tags: [kmm, architecture-driven, workflow-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# byteground/Ghostly — claude-md

**Why it's worth keeping:** Includes explicit step-by-step instructions for adding features/API changes and critical 'Common Pitfalls' that act as guardrails. The module structure breakdown is highly effective for directing AI file creation.

**Summary:** Provides comprehensive architectural context and specific development workflows for a Kotlin Multiplatform project.

**Source credibility:** Small open-source project (14 stars) with high-quality, structured documentation suggesting a professional developer.

**Recency:** Very current; uses Kotlin 2.0 and modern mobile architecture patterns.

**Source:** [byteground/Ghostly/CLAUDE.md](https://github.com/byteground/Ghostly/blob/2c33f06abd2709ce940a3385d026c8ea7e5cdb3d/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Ghostly is a Kotlin Multiplatform Mobile (KMM) application that serves as a modern, read-only client for Ghost CMS. The project demonstrates an offline-first approach with local caching and pagination support.

## Commands

### Build Commands
```bash
# Build Android app
./gradlew :androidApp:assembleDebug

# Build shared module
./gradlew :shared:build

# Clean build
./gradlew clean

# Sync iOS dependencies (run after shared module changes)
cd iosApp && pod install
```

### Development Commands
```bash
# Run Android app (requires Android Studio or connected device)
./gradlew :androidApp:installDebug

# Generate database schema (after Room entity changes)
./gradlew :shared:kspCommonMainKotlinMetadata

# Check for dependency updates
./gradlew dependencyUpdates
```

### Testing Commands
**Note:** No testing infrastructure is currently configured. When implementing tests:
- Use JUnit5 for unit tests
- MockK for mocking
- Turbine for testing Flows
- Add test commands here once configured

### Linting Commands
**Note:** No linting tools are currently co
```

</details>
