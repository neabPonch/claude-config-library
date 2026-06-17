---
name: jvm-skills__jvm-skills__photoquest-claude
source: https://github.com/jvm-skills/jvm-skills/blob/6ae5acb462ab2764e56b904cfbd830c868a81cde/examples/photoquest-CLAUDE.md
repo: jvm-skills/jvm-skills
kind: claude-md
stars: 107
last_pushed: 2026-04-30T10:26:45Z
license: apache-2.0
score: 9
domains: [backend, jvm, spring-boot]
tags: [kotlin, mcp-orchestration, workflow-management]
curated: 2026-06-15
curated_by: config-scout
---

# jvm-skills/jvm-skills — claude-md

**Why it's worth keeping:** It provides precise build/test commands, orchestrates specialized MCPs for refactoring and documentation, and mandates a 'plan-first' workflow to prevent agent drift.

**Summary:** A high-density configuration for a JVM/Spring Boot project that integrates specific MCP tool usage and strict architectural enforcement.

**Source credibility:** High; the file is exceptionally well-structured and comes from an active repository.

**Recency:** Very current, featuring modern dependencies like Tailwind v4 and specific Claude Code MCP tool patterns.

**Source:** [jvm-skills/jvm-skills/examples/photoquest-CLAUDE.md](https://github.com/jvm-skills/jvm-skills/blob/6ae5acb462ab2764e56b904cfbd830c868a81cde/examples/photoquest-CLAUDE.md) · 107★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.
## Critical Rules

- **Be extremely concise** in all interactions, plans, and commit messages. Sacrifice grammar for concision.
- **No legacy commentary**: when changing or replacing behavior, just write the new state. Never add comments explaining what was removed, what used to work, or why the old approach was replaced.
- **Compile after .kt changes**: `./gradlew compileKotlin compileTestKotlin detekt` — quiet/plain output is configured in `gradle.properties`; only errors/violations are shown.
- **Restart app after code changes**: use the `/restart` skill before verifying in the browser.
- **DB changes → migration first**: when planning, the first phase must be "Workflow for Database Migration"
- **All user-visible text in German. All developer-facing content (plans, docs, commits, comments) in English.**
- **When writing migrations use the design-postgres-table skill**
- **Use the `/test` skill to run tests** — accepts filter patterns: `/test *SetupTest *LobbyTest`.
- **Multi-instance safe**: no in-memory state for dedup/guards; use DB checks. Use `AdvisoryLock.kt`
```

</details>
