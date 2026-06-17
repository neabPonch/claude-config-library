---
name: Hyve-IDE__Hyve
source: https://github.com/Hyve-IDE/Hyve/blob/8942ed262d8f298196a99f227508ad721188bed6/CLAUDE.md
repo: Hyve-IDE/Hyve
kind: claude-md
stars: 12
last_pushed: 2026-03-22T21:35:07Z
license: apache-2.0
score: 9
domains: [ide-plugin, kotlin, jvm]
tags: [architecture-invariants, test-guidance, workflow-control]
curated: 2026-06-15
curated_by: config-scout
---

# Hyve-IDE/Hyve — claude-md

**Why it's worth keeping:** Excellent use of architectural invariants and highly specific testing/UI guidelines that preempt common LLM errors. It also defines a clear, multi-stage workflow for feature development.

**Summary:** Provides deep architectural constraints and specific technical nuances to prevent incorrect implementations in a complex IntelliJ plugin environment.

**Source credibility:** The high density of technical constraints suggests a professionally engineered codebase.

**Recency:** Very current; integrates modern agentic workflows like MCP and structured skill usage.

**Source:** [Hyve-IDE/Hyve/CLAUDE.md](https://github.com/Hyve-IDE/Hyve/blob/8942ed262d8f298196a99f227508ad721188bed6/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Hyve

IntelliJ platform plugin for Hytale game modding, consisting of three sub-systems: a core knowledge library, an IDE plugin, and a standalone MCP server.

## Files

| File | What | When to read |
| ---- | ---- | ------------ |
| `hyve-plugin/build.gradle.kts` | Standalone launcher build config | Modifying launcher packaging or bundled plugin list |
| `hyve-plugin/settings.gradle.kts` | Root settings including all plugin modules | Adding/removing modules, understanding module graph |

## Subdirectories

| Directory | What | When to read |
| --------- | ---- | ------------ |
| `plugins/hyve-common/` | Shared utilities: settings UI, Hytale install path detection, version detection | Modifying settings, adding common utilities |
| `plugins/hyve-knowledge/core/` | Core knowledge library — no IntelliJ deps; shared by IDE plugin and MCP server | Modifying indexers, search, embedding, config, or DB |
| `plugins/hyve-knowledge/src/` | IDE plugin bridge — connects core to IntelliJ services via *Factory and *Bridge classes | Adding IDE-specific features, modifying tool window |
| `plugins/hyve-knowledge/mcp-server/` | Standalone MCP server process — uses McpConfig with env var override
```

</details>
