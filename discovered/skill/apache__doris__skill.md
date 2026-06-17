---
name: apache__doris__skill
source: https://github.com/apache/doris/blob/ca4af95e2c7bfbb875d4e9d0ee01c7a1b0c43c61/.claude/skills/clang-tidy-check/SKILL.md
repo: apache/doris
kind: skill
stars: 15476
last_pushed: 2026-06-16T05:29:14Z
license: apache-2.0
score: 9
domains: [cpp, static-analysis, build-systems]
tags: [clang-tidy, cmake, cpp, quality-assurance]
curated: 2026-06-16
curated_by: config-scout
---

# apache/doris — skill

**Why it's worth keeping:** It solves the 'environmental context' problem by explaining how to generate compilation databases and providing strategies to filter noise using git diffs.

**Summary:** Automates clang-tidy static analysis for C++ files within a complex multi-module build environment.

**Source credibility:** Highly credible; Apache Doris is a major, high-starred open-source database project.

**Recency:** Current; it addresses specific developer hurdles like compile_commands.json which are highly relevant for modern AI agents.

**Source:** [apache/doris/.claude/skills/clang-tidy-check/SKILL.md](https://github.com/apache/doris/blob/ca4af95e2c7bfbb875d4e9d0ee01c7a1b0c43c61/.claude/skills/clang-tidy-check/SKILL.md) · 15476★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: clang-tidy-check
description: Run clang-tidy on newly added/modified BE C++ code
compatibility: opencode
---

## What I do

Run clang-tidy static analysis on newly added or modified C++ files in the BE and Cloud modules, using the project's `.clang-tidy` configuration. The script parses `git diff` to identify changed line ranges and filters clang-tidy output to diagnostics on those lines where possible, reducing noise from pre-existing code. Diagnostics from included headers that were not part of the diff are filtered out, though some edge cases may still appear.

## When to use me

- After building BE, before committing C++ code changes
- When CI reports clang-tidy warnings on your PR
- When you want to proactively check new code for common bugs and style issues

## Prerequisites

1. **The relevant module must be built first** — clang-tidy needs `compile_commands.json` generated during the CMake build. For BE files, build BE; for Cloud files, build Cloud.
2. **clang-tidy must be installed** — the project uses clang-tidy from the LDB toolchain.

## Procedure

### Step 1: Build the relevant module (if not already done)

For **BE** files:
```bash
./build.sh --be -j${DORIS_P
```

</details>
