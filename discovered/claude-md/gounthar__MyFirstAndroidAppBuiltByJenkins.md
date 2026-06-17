---
name: gounthar__MyFirstAndroidAppBuiltByJenkins
source: https://github.com/gounthar/MyFirstAndroidAppBuiltByJenkins/blob/2e093751d1ebf4ad921a31fdb8b776daeacd5db4/CLAUDE.md
repo: gounthar/MyFirstAndroidAppBuiltByJenkins
kind: claude-md
stars: 19
last_pushed: 2026-06-08T20:27:00Z
license: mit
score: 8
domains: [mobile-android, devops, ci-cd]
tags: [android, gradle, jenkins, docker, kotlin]
curated: 2026-06-15
curated_by: config-scout
---

# gounthar/MyFirstAndroidAppBuiltByJenkins — claude-md

**Why it's worth keeping:** It provides exhaustive, copy-pasteable Gradle commands for every stage (build, test, lint) and explicitly documents environment variable requirements crucial for infrastructure setup.

**Summary:** A comprehensive technical manual detailing the build, test, and deployment lifecycle of an Android application integrated with Jenkins/Docker CI/CD.

**Source credibility:** Moderate; it is a specialized demonstration repository with 19 stars.

**Recency:** 

**Source:** [gounthar/MyFirstAndroidAppBuiltByJenkins/CLAUDE.md](https://github.com/gounthar/MyFirstAndroidAppBuiltByJenkins/blob/2e093751d1ebf4ad921a31fdb8b776daeacd5db4/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mobile Development Documentation

This file provides guidance when working with code in this repository.

## Project Overview

This is an Android application built with Kotlin that demonstrates continuous integration and deployment using Jenkins. The project includes both the Android app source code and a complete Jenkins infrastructure for building, testing, and deploying the app to GitHub and Google Play Store.

## Build Commands

### Basic Gradle Commands

```bash
# Make gradlew executable (required on first use)
chmod +x ./gradlew

# Build the entire project
./gradlew build

# Build APKs and AABs
./gradlew :app:bundleDebug :app:bundleRelease

# Run unit tests
./gradlew test

# Run instrumented (Android) tests
./gradlew connectedAndroidTest

# Generate code coverage report
./gradlew jacocoTestReport
```

### Static Analysis

```bash
# Run Detekt with auto-correction
./gradlew detekt --auto-correct

# Run all checks (includes lint, SpotBugs, PMD, Detekt)
./gradlew check
```

### Clean Build

```bash
./gradlew clean build
```

## Jenkins Infrastructure

### Starting Jenkins Locally

The repository contains a self-contained Jenkins setup in the `jenkins/` directory.

**On Linux/M
```

</details>
