---
name: erupts__erupt
source: https://github.com/erupts/erupt/blob/e725556dd41659c0d1ef9d4bf4dfbdffbe6c3936/CLAUDE.md
repo: erupts/erupt
kind: claude-md
stars: 2739
last_pushed: 2026-06-14T13:47:41Z
license: apache-2.0
score: 9
domains: [java, backend-framework, low-code, ai-integration]
tags: [maven, spring-boot, architecture-patterns, annotation-driven]
curated: 2026-06-15
curated_by: config-scout
---

# erupts/erupt — claude-md

**Why it's worth keeping:** It explains the project's mental model (annotation-to-UI flow) and identifies specific extension points and technical gotchas like GSON usage. This allows an LLM to understand how to extend the system rather than just navigating it.

**Summary:** Provides comprehensive build commands and a deep architectural breakdown of the low-code framework's design patterns.

**Source credibility:** High; the repository is popular with 2700+ stars and shows very recent activity.

**Recency:** Highly current, including modern AI/MCP integration details.

**Source:** [erupts/erupt/CLAUDE.md](https://github.com/erupts/erupt/blob/e725556dd41659c0d1ef9d4bf4dfbdffbe6c3936/CLAUDE.md) · 2739★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Test Commands

```bash
# Build entire project
mvn clean install

# Build a single module (and its dependencies)
mvn clean install -pl erupt-core -am

# Skip tests for faster builds
mvn clean install -DskipTests

# Run all tests (erupt-test module uses H2 in-memory DB)
mvn test -pl erupt-test

# Run a specific test class
mvn test -pl erupt-test -Dtest=EruptTest

# Run a specific test method
mvn test -pl erupt-test -Dtest=EruptTest#modules

# Run the sample application for local testing
cd erupt-sample && mvn spring-boot:run

# Release build (GPG signing, Javadoc, publishes to Maven Central)
mvn clean package -P release

# Update all module versions
mvn versions:set -DnewVersion=x.x.x
```

Java 17 required. No Maven wrapper — use system `mvn`.

## Architecture Overview

Erupt is a **low-code platform framework** that auto-generates admin UIs from Java annotations, with zero frontend code required.

### Module Structure

The project is a multi-module Maven project (~25 modules):

| Group | Modules |
|-------|---------|
| Core | `erupt-annotation` (annotation
```

</details>
