---
name: kousen__java_8_recipes
source: https://github.com/kousen/java_8_recipes/blob/1171264a61e6358d66c1fdc293dd0780bb83df1f/CLAUDE.md
repo: kousen/java_8_recipes
kind: claude-md
stars: 391
last_pushed: 2026-05-13T13:19:24Z
license: unknown
score: 9
domains: [java, build-systems, testing]
tags: [junit5-migration, gradle, modernization]
curated: 2026-06-14
curated_by: config-scout
---

# kousen/java_8_recipes — claude-md

**Why it's worth keeping:** The 'Important Notes for Claude' section offers specific syntax constraints to prevent regressions, while the migration guide acts as an actionable procedural playbook for AI refactoring tasks.

**Summary:** Provides technical context, build commands, and strict rules for maintaining a modernized Java/Gradle project.

**Source credibility:** High; based on an O'Reilly book repository with recent maintenance activity.

**Recency:** Very current; uses Java 17 and modern Gradle/JUnit versions.

**Source:** [kousen/java_8_recipes/CLAUDE.md](https://github.com/kousen/java_8_recipes/blob/1171264a61e6358d66c1fdc293dd0780bb83df1f/CLAUDE.md) · 391★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Documentation

This document contains important information for Claude AI assistant when working on this project.

## Project Overview

This is the source code repository for "Modern Java Recipes" (O'Reilly, 2017). It's a Java project showcasing Java 8+ features and patterns, recently modernized with current tooling and testing frameworks.

## Build System & Dependencies

### Core Technologies
- **Language**: Java 17 (using Gradle toolchain)
- **Build Tool**: Gradle 8.14.2 (latest stable)
- **Testing**: JUnit 5.13.2 (fully migrated from JUnit 4)
- **CI**: GitHub Actions

### Key Dependencies
- `org.junit.jupiter:junit-jupiter` - Main testing framework
- `org.junit.platform:junit-platform-launcher` - Required for test execution
- `org.mockito:mockito-junit-jupiter` - Mocking framework
- `org.assertj:assertj-core` - Fluent assertions
- JMH for benchmarking tests

### Dependency Management
- Uses Gradle version catalogs (`gradle/libs.versions.toml`)
- JUnit BOM manages all JUnit component versions consistently
- No JUnit vintage engine (fully migrated to JUnit 5)

## Project Structure

```
src/
├── main/java/          # Main source code with Java 8+ examples
├── t
```

</details>
