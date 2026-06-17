---
name: vicwomg__pikaraoke
source: https://github.com/vicwomg/pikaraoke/blob/c406a10f2fd154e2d4f5c75b39f57f511f6772f3/CLAUDE.md
repo: vicwomg/pikaraoke
kind: claude-md
stars: 833
last_pushed: 2026-05-19T21:35:18Z
license: unknown
score: 9
domains: [python, iot]
tags: [opinionated, refactoring, domain-specific]
curated: 2026-06-15
curated_by: config-scout
---

# vicwomg/pikaraoke — claude-md

**Why it's worth keeping:** The 'when to refactor' logic (Rule of Three) and the exact YouTube filename pattern constraints are highly effective at preventing AI over-engineering and errors.

**Summary:** Provides strict engineering principles, refactoring heuristics, and specific domain-specific file naming patterns for a Python/YouTube project.

**Source credibility:** High; from an active, well-starred open-source repository.

**Recency:** Current; utilizes modern Python 3.10+ syntax and 'uv' toolchain standards.

**Source:** [vicwomg/pikaraoke/CLAUDE.md](https://github.com/vicwomg/pikaraoke/blob/c406a10f2fd154e2d4f5c75b39f57f511f6772f3/CLAUDE.md) · 833★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code when working on PiKaraoke.

## Project Overview

PiKaraoke is a karaoke system for Raspberry Pi, Windows, macOS, and Linux. Web interface for YouTube song search, queuing, and playback with pitch shifting and streaming.

## Core Principles

**Single-owner maintainability:** Code clarity over documentation. Simplicity over flexibility. One source of truth.

## Refactoring

**Refactor iteratively as you work.** When touching code:

- Extract classes when a module has multiple responsibilities (like `Browser` was extracted from utilities)
- Extract functions when logic is repeated or a function exceeds ~50 lines
- Rename unclear variables/functions immediately
- Delete dead code - never comment it out. When new code supersedes existing methods, remove the old methods and their tests in the same commit
- Update related code consistently (no half-migrations)

**When to refactor:**

- Code you're modifying is hard to understand
- You're adding a third similar pattern (rule of three)
- A function/class is doing too many things

**When NOT to refactor:**

- Unrelated code "while you're in the area"
- Working code that you're not modifying
- To add flex
```

</details>
