---
name: omnimind-ai__OpenOmniBot
source: https://github.com/omnimind-ai/OpenOmniBot/blob/96750b5cc3d9d8f3a5112d01f32e0efa4be01974/CLAUDE.md
repo: omnimind-ai/OpenOmniBot
kind: claude-md
stars: 1706
last_pushed: 2026-06-14T22:58:04Z
license: other
score: 9
domains: [android-development, flutter, mobile-apps, ai-agents]
tags: [hybrid-app, gradle, riverpod, architecture-guide]
curated: 2026-06-14
curated_by: config-scout
---

# omnimind-ai/OpenOmniBot — claude-md

**Why it's worth keeping:** Exceptional breakdown of dual-stack commands (Gradle vs. Flutter) and clear explanations of architectural patterns like the State Machine and module integration logic.

**Summary:** A comprehensive guide for a complex hybrid Android and Flutter project, detailing multi-module interactions and build environments.

**Source credibility:** High; popular repository with 1706 stars and active maintenance.

**Recency:** Current; includes modern Android/Flutter context and MCP integration notes.

**Source:** [omnimind-ai/OpenOmniBot/CLAUDE.md](https://github.com/omnimind-ai/OpenOmniBot/blob/96750b5cc3d9d8f3a5112d01f32e0efa4be01974/CLAUDE.md) · 1706★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OmnibotApp is an AI-powered intelligent robot assistant application for Android. It's a hybrid app combining native Android Kotlin code with Flutter UI, implementing a modular architecture with clear separation of concerns.

**Key characteristics:**
- Android app with embedded Flutter UI module
- Modular monorepo architecture with feature-specific modules
- State machine-based task management system
- Accessibility services and overlay functionality
- AI/ML intelligence integration (on-device models)

## Build and Development Commands

### Android/Gradle Commands
```bash
# Full project build
./gradlew build

# Build debug APK (develop flavor)
./gradlew assembleDevelopDebug

# Build release APK (production flavor)
./gradlew assembleProductionRelease

# Run tests
./gradlew test

# Run instrumented tests
./gradlew connectedAndroidTest

# Lint checking
./gradlew lint

# Install debug APK to connected device
./gradlew installDevelopDebug
```

### Flutter Commands (for ui/ module)
```bash
cd ui

# Install dependencies
flutter pub get

# If you encounte
```

</details>
