---
name: utopia-rise__godot-kotlin-jvm
source: https://github.com/utopia-rise/godot-kotlin-jvm/blob/4ebf9c7a631e91689250c50b98c7d824cd249eda/CLAUDE.md
repo: utopia-rise/godot-kotlin-jvm
kind: claude-md
stars: 929
last_pushed: 2026-06-08T01:25:32Z
license: mit
score: 10
domains: [game-engine, native-integration, jvm]
tags: [hybrid-build, debugging-guide, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# utopia-rise/godot-kotlin-jvm — claude-md

**Why it's worth keeping:** Includes specific troubleshooting/debugging commands for deep processes (KSP) and explicit warnings about environment-specific failures like the Microsoft JDK issue.

**Summary:** Provides comprehensive technical context for a complex hybrid C++/JVM project, covering multiple build systems and environmental quirks.

**Source credibility:** Highly credible; a well-maintained, high-star repository in the Godot ecosystem.

**Recency:** Current; includes up-to-date versioning and modern build/debug workflows.

**Source:** [utopia-rise/godot-kotlin-jvm/CLAUDE.md](https://github.com/utopia-rise/godot-kotlin-jvm/blob/4ebf9c7a631e91689250c50b98c7d824cd249eda/CLAUDE.md) · 929★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Is

**Godot-JVM** is a Godot engine module that enables Kotlin (and Java/Scala) as scripting languages. It is a hybrid C++/JVM project: the C++ side integrates with Godot's module system, and the Kotlin/Gradle side provides the runtime libraries and tooling for user projects.

Current binding version: `0.16.2` targeting Godot `4.6.3`.

## Prerequisites

- **JDK 17+** required for building IDE/Gradle plugins (JDK 11+ for runtime-only builds)
- Use **Adoptium/Eclipse Temurin** JDK — Microsoft JDK causes IDE plugin build failures (known issue [microsoft/openjdk#339](https://github.com/microsoft/openjdk/issues/339)). If you must use Microsoft JDK, manually create the `Packages` folder inside `JAVA_HOME`.
- `JAVA_HOME` must be set
- Standard Godot build deps: SCons, Python, C++ compiler

## Build Commands

The project has two independent build systems that must both be built.

### C++ Module (SCons)

This module lives as a submodule at `modules/kotlin_jvm/` inside the Godot source tree. All SCons commands run from the **Godot source root**.

```bash
s
```

</details>
