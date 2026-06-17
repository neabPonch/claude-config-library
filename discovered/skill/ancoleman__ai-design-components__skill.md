---
name: ancoleman__ai-design-components__skill
source: https://github.com/ancoleman/ai-design-components/blob/76551b7b19ebc667764ec75da14990d0aef8b6e5/skills/shell-scripting/SKILL.md
repo: ancoleman/ai-design-components
kind: skill
stars: 374
last_pushed: 2025-12-11T00:50:33Z
license: mit
score: 9
domains: [cli-tools, devops, automation]
tags: [shell, bash, scripting, devops]
curated: 2026-06-16
curated_by: config-scout
---

# ancoleman/ai-design-components — skill

**Why it's worth keeping:** Includes essential patterns like 'set -euo pipefail', trap-based cleanup, and a complete production script template that prevents common scripting pitfalls.

**Summary:** A high-quality instruction set for writing production-grade shell scripts with a focus on reliability and portability.

**Source credibility:** Strong; 374 stars indicates high utility and the depth of specific shell edge cases suggests expert authorship.

**Recency:** Highly current, incorporating modern tool patterns like yq v4 and container-optimized practices.

**Source:** [ancoleman/ai-design-components/skills/shell-scripting/SKILL.md](https://github.com/ancoleman/ai-design-components/blob/76551b7b19ebc667764ec75da14990d0aef8b6e5/skills/shell-scripting/SKILL.md) · 374★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: shell-scripting
description: Write robust, portable shell scripts with proper error handling, argument parsing, and testing. Use when automating system tasks, building CI/CD scripts, or creating container entrypoints.
---

# Shell Scripting

## Purpose

Provides patterns and best practices for writing maintainable shell scripts with error handling, argument parsing, and portability considerations. Covers POSIX sh vs Bash decision-making, parameter expansion, integration with common utilities (jq, yq, awk), and testing with ShellCheck and Bats.

## When to Use This Skill

Use shell scripting when:
- Orchestrating existing command-line tools and system utilities
- Writing CI/CD pipeline scripts (GitHub Actions, GitLab CI)
- Creating container entrypoints and initialization scripts
- Automating system administration tasks (backups, log rotation)
- Building development tooling (build scripts, test runners)

Consider Python/Go instead when:
- Complex business logic or data structures required
- Cross-platform GUI needed
- Heavy API integration (REST, gRPC)
- Script exceeds 200 lines with significant logic complexity

## POSIX sh vs Bash

**Use POSIX sh (#!/bin/sh) when:**
- Ma
```

</details>
