---
name: mikepenz__AboutLibraries
source: https://github.com/mikepenz/AboutLibraries/blob/f388cb11cca6eb33bb358c3b849a5bae0cc47735/CLAUDE.md
repo: mikepenz/AboutLibraries
kind: claude-md
stars: 4336
last_pushed: 2026-06-14T23:00:53Z
license: apache-2.0
score: 9
domains: [mobile, kotlin-multiplatform, android]
tags: [kmp, gradle, build-automation, conventional-commits]
curated: 2026-06-15
curated_by: config-scout
---

# mikepenz/AboutLibraries — claude-md

**Why it's worth keeping:** Excellent use of context-specific build instructions (directory-aware) and highly specific, structured rules for dependency update commit messages.

**Summary:** Provides comprehensive context for a multi-module Kotlin Multiplatform project, distinguishing between main project and plugin commands.

**Source credibility:** Highly credible; the repository is a popular, widely-used library with active maintenance.

**Recency:** Very recent and aligned with modern Kotlin/Gradle development standards.

**Source:** [mikepenz/AboutLibraries/CLAUDE.md](https://github.com/mikepenz/AboutLibraries/blob/f388cb11cca6eb33bb358c3b849a5bae0cc47735/CLAUDE.md) · 4336★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

AboutLibraries is a **Kotlin Multiplatform (KMP)** library that automatically collects dependency and license information from Gradle projects at build time (via a Gradle plugin) and provides Compose/View-based UI to display it at runtime.

The Gradle plugin lives in a **separate Gradle build** under `plugin-build/`. The main project and `plugin-build/` are independent Gradle projects — commands for one do not apply to the other.

## Common Commands

### Main Project
```bash
./gradlew build                                          # Build all modules
./gradlew lintDebug                                      # Lint Android modules
./gradlew apiCheck                                       # Binary compatibility validation
./gradlew :sample:android:assembleDebug                  # Build Android sample
./gradlew :sample:android:verifyPaparazziDebug           # Run Paparazzi screenshot tests
./gradlew :sample:android:recordPaparazziDebug           # Update (record) screenshot baselines
./gradlew :sample:desktop:run                            # Run desktop sampl
```

</details>
