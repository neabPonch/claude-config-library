---
name: bbfox0703__UE5CEDumper
source: https://github.com/bbfox0703/UE5CEDumper/blob/0c573c83f804d48dddb3d8a7f22f57fd1a2ffc00/Claude.MD
repo: bbfox0703/UE5CEDumper
kind: claude-md
stars: 23
last_pushed: 2026-06-16T03:06:58Z
license: mit
score: 9
domains: [systems-programming, game-dev, security-tools]
tags: [low-level, build-automation, architecture-map, strict-rules]
curated: 2026-06-16
curated_by: config-scout
---

# bbfox0703/UE5CEDumper — claude-md

**Why it's worth keeping:** The 'Unified Build Script' pattern (explaining environmental dependencies) and the comprehensive architectural overview are elite techniques. The specific rules regarding platform abstraction and AOT compatibility provide excellent guardrails for high-performance code.

**Summary:** Provides rigorous technical guardrails and a highly detailed structural map for a complex low-level C++/C# project. It excels at defining environment-specific build requirements to prevent tool failure.

**Source credibility:** High; a specialized, active utility with recent development history.

**Recency:** Very current; incorporates modern C# constraints like Native AOT/Source Generators.

**Source:** [bbfox0703/UE5CEDumper/Claude.MD](https://github.com/bbfox0703/UE5CEDumper/blob/0c573c83f804d48dddb3d8a7f22f57fd1a2ffc00/Claude.MD) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> For detailed specs, implementation history, and debugging notes, see the **[docs/](docs/)** directory.

-----

## Build & Deploy
- After making code changes, always do a full rebuild and verify the build output is actually updated before testing. Never assume a build succeeded without checking.

-----

## Code Changes
- When asked to refactor or rename modules/files, make actual code changes (move files, update imports, rename classes) — not just documentation updates. Confirm structural changes before proceeding to docs.

-----

## Debugging
- When fixing bugs, verify the fix against the actual memory layout or data structure rather than assuming. If the first fix doesn't work, re-examine fundamental assumptions about the data format before iterating.

-----

## Git Operations
- When creating PRs, check for branch divergence and resolve merge conflicts before attempting `gh pr create`. Run `git status` and `git log --oneline -5` first.

-----

## Cheat Engine
- When working with CE Lua APIs, verify that functions/methods actually exist in the Cheat Engine Lua API
```

</details>
