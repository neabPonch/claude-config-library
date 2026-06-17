---
name: minigdx__tiny
source: https://github.com/minigdx/tiny/blob/876365cfc867ea64f89e6df5d809aadc8913f370/CLAUDE.md
repo: minigdx/tiny
kind: claude-md
stars: 159
last_pushed: 2026-05-28T12:35:10Z
license: mit
score: 9
domains: [game-engine, graphics-programming, cli-tools]
tags: [kotlin, lua, opengl, multiplatform]
curated: 2026-06-17
curated_by: config-scout
---

# minigdx/tiny — claude-md

**Why it's worth keeping:** Includes deep technical specifics like OpenGL rendering stages and platform-specific performance pitfalls that are critical for preventing common architectural errors.

**Summary:** A highly detailed guide detailing a Kotlin Multiplatform engine's architecture, rendering stages, and specific development workflows.

**Source credibility:** High; the repository is well-maintained with significant community interest (159 stars).

**Recency:** Current; reflects modern Kotlin Multiplatform and Gradle workflows.

**Source:** [minigdx/tiny/CLAUDE.md](https://github.com/minigdx/tiny/blob/876365cfc867ea64f89e6df5d809aadc8913f370/CLAUDE.md) · 159★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Architecture Overview

Tiny is a Kotlin Multiplatform game engine with Lua scripting support that compiles to desktop (JVM) and web (JavaScript) platforms. The project is structured as a multi-module Gradle build:

- **tiny-engine**: Core multiplatform game engine (commonMain, jvmMain, jsMain)
- **tiny-cli**: JVM-based CLI tool for development workflows
- **tiny-doc**: Documentation generation using Asciidoctor
- **tiny-doc-annotations**: Annotations for documentation generation
- **tiny-doc-generator**: KSP-based documentation processor
- **tiny-web-editor**: Web-based editor interface
- **tiny-samples**: Sample games and examples

## Key Technologies

- **Kotlin Multiplatform**: Shared code between JVM and JS platforms
- **Lua**: Game scripting via luak library
- **OpenGL**: Graphics rendering via kgl and LWJGL
- **Ktor**: HTTP server for CLI serve command
- **KSP**: Documentation generation from code annotations

## Development Commands

### Building
```bash
./gradlew build                    # Build all modules
./gradlew test                     # Run all test
```

</details>
