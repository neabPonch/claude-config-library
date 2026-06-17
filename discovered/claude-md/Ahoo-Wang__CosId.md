---
name: Ahoo-Wang__CosId
source: https://github.com/Ahoo-Wang/CosId/blob/514a9e96b88e09936203162a707e1da300279743/CLAUDE.md
repo: Ahoo-Wang/CosId
kind: claude-md
stars: 630
last_pushed: 2026-05-28T15:14:10Z
license: apache-2.0
score: 9
domains: [backend, distributed-systems, java]
tags: [gradle, java, performance]
curated: 2026-06-16
curated_by: config-scout
---

# Ahoo-Wang/CosId — claude-md

**Why it's worth keeping:** Includes critical low-level technical details like JVM --add-opens flags, specific import ordering rules, and complex module dependency mappings that prevent AI errors.

**Summary:** Provides deep architectural context, comprehensive build instructions including benchmarks, and strict development environment constraints.

**Source credibility:** High; the repository is a well-starred open-source project with recent maintenance.

**Recency:** Current; utilizes modern Java 17 features and Gradle Version Catalogs.

**Source:** [Ahoo-Wang/CosId/CLAUDE.md](https://github.com/Ahoo-Wang/CosId/blob/514a9e96b88e09936203162a707e1da300279743/CLAUDE.md) · 630★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CosId is a universal, flexible, high-performance distributed ID generator for Java 17+. It provides several ID generation strategies:

- **CosIdGenerator**: Standalone high-performance ID generator (~15M+ ops/s)
- **SnowflakeId**: 64-bit distributed ID with machine ID allocation and clock sync
- **SegmentId**: Batch ID allocation to reduce network IO
- **SegmentChainId**: Lock-free enhancement of SegmentId (~127M+ ops/s)

## Build Commands

```bash
# Build entire project
./gradlew build

# Build specific module
./gradlew :cosid-core:build

# Run all tests
./gradlew test

# Run single test class
./gradlew :cosid-core:test --tests "me.ahoo.cosid.snowflake.MillisecondSnowflakeIdTest"

# Run single test method
./gradlew :cosid-core:test --tests "me.ahoo.cosid.snowflake.MillisecondSnowflakeIdTest.generate"

# Lint/Check (Checkstyle + SpotBugs)
./gradlew check

# Run JMH benchmark (all)
./gradlew :cosid-core:jmh

# Run JMH benchmark (filtered by class name)
./gradlew :cosid-core:jmh -PjmhIncludes=SnowflakeIdBenchmark

# Run Spring Boot example
./gradle
```

</details>
