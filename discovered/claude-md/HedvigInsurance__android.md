---
name: HedvigInsurance__android
source: https://github.com/HedvigInsurance/android/blob/616b1bd9c7208696d938a709222c36471cb6b107/CLAUDE.md
repo: HedvigInsurance/android
kind: claude-md
stars: 149
last_pushed: 2026-06-13T14:05:42Z
license: agpl-3.0
score: 9
domains: [android, mobile-dev, kotlin]
tags: [architecture, mvi, graphql, modularization, jetpack-compose]
curated: 2026-06-15
curated_by: config-scout
---

# HedvigInsurance/android — claude-md

**Why it's worth keeping:** It includes strict 'critical architectural rules' that prevent common errors like leaking GraphQL types or illegal module dependencies, alongside specific code patterns for state management.

**Summary:** A highly detailed guide for a large-scale modular Android project using MVI with Molecule and Apollo GraphQL.

**Source credibility:** High-quality professional repository with active maintenance and significant star count.

**Recency:** Very current; utilizes modern Android practices like Jetpack Compose, KMP, and type-safe navigation.

**Source:** [HedvigInsurance/android/CLAUDE.md](https://github.com/HedvigInsurance/android/blob/616b1bd9c7208696d938a709222c36471cb6b107/CLAUDE.md) · 149★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Hedvig Android app - A modern Android application built with Jetpack Compose, Apollo GraphQL, and Kotlin. The app uses a highly modular architecture with 80+ modules organized into feature, data, and core layers.

## Essential Setup Commands

### Initial Setup
```bash
# 1. Download GraphQL schema (required before building)
./gradlew downloadOctopusApolloSchemaFromIntrospection

# 2. Download translations from Lokalise (required before building)
./gradlew downloadStrings

# 3. Build and sync the project
./gradlew build
```

**Prerequisites:**
- `lokalise.properties` file with credentials (from 1Password)
- `~/.gradle/gradle.properties` with GitHub Packages token (PAT with `read:packages` permission)
- See `scripts/ci-prebuild.sh` for reference

### Common Development Commands

```bash
# Build the app
./gradlew :app:assemble

# Run all tests
./gradlew test

# Run tests for a specific module
./gradlew :feature-home:test

# Run unit tests
./gradlew testDebugUnitTest

# Formatting
./gradlew ktlintCheck          # Check formatting
./gradlew ktlintFormat
```

</details>
