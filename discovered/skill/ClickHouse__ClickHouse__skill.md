---
name: ClickHouse__ClickHouse__skill
source: https://github.com/ClickHouse/ClickHouse/blob/c3be9310ee8c2af93f00b16941e14b900ff3796c/.claude/skills/update-contrib/SKILL.md
repo: ClickHouse/ClickHouse
kind: skill
stars: 48024
last_pushed: 2026-06-16T05:27:08Z
license: apache-2.0
score: 9
domains: [devops, build-systems, infrastructure]
tags: [git-submodules, cmake, rust, dependency-management]
curated: 2026-06-16
curated_by: config-scout
---

# ClickHouse/ClickHouse — skill

**Why it's worth keeping:** It implements a rigorous 'audit-before-apply' pattern, using file tree diffing to detect necessary CMake or Rust integration changes caused by version bumps.

**Summary:** A specialized orchestration skill for managing third-party dependency updates via git submodules within the ClickHouse build system.

**Source credibility:** Highly credible; originates from the official ClickHouse repository, a widely used industry-standard database.

**Recency:** Current; utilizes sophisticated Git workflows and modern build system patterns (CMake/Rust) compatible with advanced agents.

**Source:** [ClickHouse/ClickHouse/.claude/skills/update-contrib/SKILL.md](https://github.com/ClickHouse/ClickHouse/blob/c3be9310ee8c2af93f00b16941e14b900ff3796c/.claude/skills/update-contrib/SKILL.md) · 48024★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: update-contrib
description: Update a ClickHouse third-party library (contrib submodule) to a new version. Handles fork management, submodule pointer bumps, CMake adaptation, and source code fixes. Use when the user wants to bump a dependency.
argument-hint: <library-name> [target-version]
disable-model-invocation: false
allowed-tools: Agent, Task, Bash, Read, Write, Edit, Glob, Grep, WebFetch, AskUserQuestion
---

# Update a ClickHouse Contrib (Third-Party Library)

Bump a git submodule under `contrib/` to a new version, adapting CMake build files and ClickHouse source code as needed.

## Arguments

- `$0` (required): Library name as it appears under `contrib/` (e.g., `curl`, `openssl`, `arrow`)
- `$1` (optional): Target version — a git tag, branch, or commit SHA. If omitted, the latest upstream release tag is used.

## Background

ClickHouse vendors all third-party libraries as git submodules under `contrib/`. Each library has:
- `contrib/<lib>/` — the submodule (upstream repo or a ClickHouse fork)
- `contrib/<lib>-cmake/` — ClickHouse's own CMake build files (upstream CMake is deleted after checkout)

Submodule URLs point to either upstream directly (unpatched) or a for
```

</details>
