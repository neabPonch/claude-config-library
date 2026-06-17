---
name: MaibornWolff__codecharta
source: https://github.com/MaibornWolff/codecharta/blob/faea7687423dc40bfa93df5ec27d3c0b8e3d4c06/CLAUDE.md
repo: MaibornWolff/codecharta
kind: claude-md
stars: 462
last_pushed: 2026-06-12T20:38:32Z
license: bsd-3-clause
score: 9
domains: [cli-tools, web-frontend, data-visualization]
tags: [multi-module, architecture-mapping, gradle, angular]
curated: 2026-06-15
curated_by: config-scout
---

# MaibornWolff/codecharta — claude-md

**Why it's worth keeping:** It includes crucial 'gotcha' warnings for directory-specific commands and maps complex data flows (Pipes & Filters) which helps the AI understand design patterns rather than just syntax.

**Summary:** An exceptional dual-stack guide that provides deep architectural context for both a Kotlin CLI and an Angular/Three.js frontend.

**Source credibility:** High; a well-maintained, popular open-source project with significant GitHub stars.

**Recency:** Highly current; includes modern framework versions like Angular 20 and specific environment requirements.

**Source:** [MaibornWolff/codecharta/CLAUDE.md](https://github.com/MaibornWolff/codecharta/blob/faea7687423dc40bfa93df5ec27d3c0b8e3d4c06/CLAUDE.md) · 462★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CodeCharta is a code visualization tool that generates 3D treemap visualizations of codebases. It consists of two main components:

- **Analysis (Kotlin/Java)**: CLI tool (`ccsh`) that parses source code, imports metrics from external tools, and generates `.cc.json` files
- **Visualization (TypeScript/Angular)**: Web and desktop application that renders `.cc.json` files as interactive 3D treemaps using Three.js

## Requirements

- Java >= 11, <= 21
- Node >= 20
- Git (with bash utilities for Windows)

## Common Development Commands

### Root Directory

```bash
# Install root dependencies (Husky, BiomeJS for formatting)
npm i

# Format all files
npm run format

# Check formatting
npm run format:check
```

### Analysis (Kotlin/Gradle)

```bash
cd analysis

# Build the project (creates distribution in build/)
./gradlew build

# Assemble without running tests (faster for frequent builds)
./gradlew assemble

# Install distribution locally for testing
./gradlew installDist

# Run all tests
./gradlew test

# Run integration tests (requires bash on Windo
```

</details>
