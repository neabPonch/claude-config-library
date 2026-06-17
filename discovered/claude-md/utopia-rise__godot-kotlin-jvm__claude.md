---
name: utopia-rise__godot-kotlin-jvm__claude
source: https://github.com/utopia-rise/godot-kotlin-jvm/blob/4ebf9c7a631e91689250c50b98c7d824cd249eda/kt/plugins/godot-intellij-plugin/CLAUDE.md
repo: utopia-rise/godot-kotlin-jvm
kind: claude-md
stars: 931
last_pushed: 2026-06-08T01:25:32Z
license: mit
score: 9
domains: [intellij-plugin, kotlin, tooling]
tags: [architecture-mapping, mental-model, onboarding]
curated: 2026-06-16
curated_by: config-scout
---

# utopia-rise/godot-kotlin-jvm — claude-md

**Why it's worth keeping:** It defines clear architectural patterns (e.g., Inspection vs. Analyzer) and provides an explicit reading order/onboarding path that prevents agent confusion during complex tasks.

**Summary:** Provides a hierarchical mental model of the plugin architecture, mapping files to functional layers and explaining their specific roles in the system lifecycle.

**Source credibility:** High; part of a specialized, high-star repository for Godot-Kotlin integration.

**Recency:** Highly current; explicitly references K2 analysis which is the latest IntelliJ standard.

**Source:** [utopia-rise/godot-kotlin-jvm/kt/plugins/godot-intellij-plugin/CLAUDE.md](https://github.com/utopia-rise/godot-kotlin-jvm/blob/4ebf9c7a631e91689250c50b98c7d824cd249eda/kt/plugins/godot-intellij-plugin/CLAUDE.md) · 931★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file explains how to work on `kt/plugins/godot-intellij-plugin`.

## Purpose

`godot-intellij-plugin` is the IntelliJ IDEA plugin for Godot Kotlin/JVM.

Its job is intentionally narrow:

1. provide editor checks for Godot Kotlin/JVM code
2. offer small quick fixes for common mistakes
3. detect whether a file belongs to a Godot project
4. create starter projects and modules from templates

Keep it Kotlin-first, K2-only, and simple.

Java and Scala support should only be kept where the same JVM-facing implementation stays clean.

## Mental Model

Think of the plugin as six small layers:

1. plugin wiring
2. startup and caches
3. project scope helpers
4. inspections
5. analyzers
6. quick fixes and wizard

### 1. Plugin wiring

The real entry point is:

- [plugin.xml](src/main/resources/META-INF/plugin.xml)

This is where IntelliJ is told about:

- project services
- startup activity
- inspections
- the new project wizard generator
- resource bundle

If it is not registered there, IntelliJ will not load it.

### 2. Startup and caches

These files live at the root package:

- [GodotKotlinJvmProjectActivity.kt](src/main/kotlin/godot/intellij/plugin/GodotKotlinJvmProject
```

</details>
