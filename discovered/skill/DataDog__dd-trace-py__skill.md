---
name: DataDog__dd-trace-py__skill
source: https://github.com/DataDog/dd-trace-py/blob/33e26579b1750384172fbd6cca64be00b461e74d/.claude/skills/lint/SKILL.md
repo: DataDog/dd-trace-py
kind: skill
stars: 642
last_pushed: 2026-06-15T06:53:22Z
license: other
score: 9
domains: [python, devops, quality-assurance]
tags: [linting, formatting, workflows, typing, security]
curated: 2026-06-15
curated_by: config-scout
---

# DataDog/dd-trace-py — skill

**Why it's worth keeping:** It teaches the agent to favor targeted file-based commands over slow full-suite checks, minimizing execution time and noise. The inclusion of 'Common Workflows' and 'Best Practices' gives the agent a clear behavioral roadmap for maintaining code quality.

**Summary:** This skill provides exhaustive documentation for a project's specific linting and quality assurance tooling. It categorizes commands by type (format, style, typing, security) with exact CLI usage patterns.

**Source credibility:** High; sourced from Datadog's official Python APM client, which is a highly maintained professional repository.

**Recency:** 

**Source:** [DataDog/dd-trace-py/.claude/skills/lint/SKILL.md](https://github.com/DataDog/dd-trace-py/blob/33e26579b1750384172fbd6cca64be00b461e74d/.claude/skills/lint/SKILL.md) · 642★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: lint
description: >
  Run targeted linting, formatting, and code quality checks on modified files.
  Use this to validate code style, type safety, security, and other quality metrics
  before committing. Supports running all checks or targeting specific checks on
  specific files for efficient validation.
allowed-tools:
  - Bash
  - Read
  - Grep
  - Glob
  - TodoWrite
---

# Linting and Code Quality Skill

This skill helps you efficiently validate and format code using the project's comprehensive linting infrastructure.

## When to Use This Skill

Use this skill when you:
- Edit a file and want to format it before committing
- Need to validate code style, types, or security
- Want to check for spelling errors or documentation issues
- Need to validate test infrastructure (suitespec, log messages)
- Want to run comprehensive quality checks before pushing

## Key Principles

1. **Always format after editing** - Use `scripts/lint fmt -- <file>` immediately after code changes
2. **Run comprehensive checks before committing** - Use `scripts/lint checks` before pushing
3. **Target specific files** - Use `-- <file>` syntax to validate only what you changed, not the entire codeb
```

</details>
