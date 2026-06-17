---
name: TencentCloudBase__CloudBase-MCP__skill
source: https://github.com/TencentCloudBase/CloudBase-MCP/blob/d671d0b4e4b5e082fe96b18ffd691843d4a9e51a/skills/pr-review-fix/SKILL.md
repo: TencentCloudBase/CloudBase-MCP
kind: skill
stars: 1035
last_pushed: 2026-06-16T05:36:02Z
license: mit
score: 8
domains: [devops, git-operations, ci-cd, automation]
tags: [github, pr-management, workflow-template]
curated: 2026-06-16
curated_by: config-scout
---

# TencentCloudBase/CloudBase-MCP — skill

**Why it's worth keeping:** The structured four-phase lifecycle (Discovery, Triage, Fix, Verify) and strict branch management protocols (stashing/local verification) provide a highly reliable blueprint for autonomous maintenance tasks.

**Summary:** An end-to-end agentic workflow for triaging and fixing open pull requests using the GitHub CLI.

**Source credibility:** High; comes from an established repository with significant star count and recent activity.

**Recency:** Current; uses modern GitHub CLI commands and standard developer workflows compatible with current agentic capabilities.

**Source:** [TencentCloudBase/CloudBase-MCP/skills/pr-review-fix/SKILL.md](https://github.com/TencentCloudBase/CloudBase-MCP/blob/d671d0b4e4b5e082fe96b18ffd691843d4a9e51a/skills/pr-review-fix/SKILL.md) · 1035★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pr-review-fix
description: Periodically analyze open pull requests for CI failures, code review feedback, and quality issues, then fix them in batch. Use this skill when the user asks to check PR status, triage CI failures, fix review comments, analyze open PRs, or run a scheduled PR health check across the repository.
alwaysApply: false
---

# PR Review & Fix

Systematically analyze open pull requests for CI failures, code review feedback, and code quality issues — then fix them efficiently.

## When to use this skill

Use this skill when you need to:

- Check the status of all open PRs (CI, reviews, conflicts)
- Triage and fix CI build/test failures on PR branches
- Address code review feedback (reviewer comments, requested changes)
- Run a scheduled health check across all open PRs
- Fix multiple PRs in a single session without losing context

**Do NOT use for:**

- Creating new PRs or new features
- Merging PRs (that's a manual decision)
- General code refactoring unrelated to PR feedback
- Reviewing code as a reviewer (this skill is for *responding* to reviews)

## Workflow

### Phase 1 — Discovery

1. Read `references/discovery.md` for the full discovery procedure.
```

</details>
