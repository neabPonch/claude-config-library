---
name: BentoBoxWorld__BentoBox
source: https://github.com/BentoBoxWorld/BentoBox/blob/f3d1f88bb1e9fd5daeeb88f5c76860657a92d2b9/CLAUDE.md
repo: BentoBoxWorld/BentoBox
kind: claude-md
stars: 403
last_pushed: 2026-06-15T14:54:11Z
license: epl-2.0
score: 9
domains: [java, game-development, api-design]
tags: [architecture, testing-patterns, pitfalls, binary-compatibility]
curated: 2026-06-15
curated_by: config-scout
---

# BentoBoxWorld/BentoBox — claude-md

**Why it's worth keeping:** Uses 'Key API Patterns' to teach by example rather than just definition, and includes a crucial section on technical debt/quirks to prevent the AI from re-introducing subtle bugs.

**Summary:** Provides deep architectural context, specific testing inheritance patterns, and explicit warnings about binary compatibility and data serialization quirks.

**Source credibility:** High; part of a popular, actively maintained Minecraft ecosystem project with hundreds of stars.

**Recency:** Extremely recent; reflects current development state and modern Java standards.

**Source:** [BentoBoxWorld/BentoBox/CLAUDE.md](https://github.com/BentoBoxWorld/BentoBox/blob/f3d1f88bb1e9fd5daeeb88f5c76860657a92d2b9/CLAUDE.md) · 403★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

BentoBox is a Bukkit/Paper library plugin (Java 21) that provides the core platform for island-style Minecraft games (SkyBlock, AcidIsland, etc.) via an extensible addon system.

## Build Commands

```bash
./gradlew build              # Build the shaded JAR
./gradlew test               # Run all tests
./gradlew clean build        # Clean then build
./gradlew jacocoTestReport   # Generate coverage report (build/reports/jacoco/)
```

### Running a Single Test

```bash
# Run all tests in a class
./gradlew test --tests "world.bentobox.bentobox.managers.IslandsManagerTest"

# Run a specific test method
./gradlew test --tests "world.bentobox.bentobox.managers.IslandsManagerTest.testMethodName"
```

## Architecture

The main plugin class is `BentoBox.java` (extends `JavaPlugin`). Almost all subsystems are accessed via singleton managers held by the plugin instance.

### Key Packages

- **`api/`** — Public API surface for addons: events, commands, panels (GUIs), user management, flags, configuration
- **`managers/`** — Core subsystems: `IslandsManager`,
```

</details>
