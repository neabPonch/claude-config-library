---
name: dderyldowney__todowrite__claude-original
source: https://github.com/dderyldowney/todowrite/blob/499d923c26bccf103218aca9dab949f998a0a641/.claude/CLAUDE.md.original
repo: dderyldowney/todowrite
kind: claude-md
stars: 3
last_pushed: 2025-11-28T02:50:13Z
license: unknown
score: 9
domains: [cli-tools, backend, security, devops]
tags: [opinionated, workflow, bootstrapping, security]
curated: 2026-06-16
curated_by: config-scout
---

# dderyldowney/todowrite — claude-md

**Why it's worth keeping:** The instruction to load documentation files in a specific order on startup is a brilliant context-management technique; the use of authoritative URL lists is also highly effective for reducing hallucinations.

**Summary:** Establishes strict architectural mandates including a zero-mocking policy, specific branch workflows, and an ordered documentation loading sequence.

**Source credibility:** Low star count but demonstrates highly intentional, opinionated engineering standards.

**Recency:** Current and highly relevant to modern agentic workflows.

**Source:** [dderyldowney/todowrite/.claude/CLAUDE.md.original](https://github.com/dderyldowney/todowrite/blob/499d923c26bccf103218aca9dab949f998a0a641/.claude/CLAUDE.md.original) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file defines **non-negotiable, permanent rules** for Claude and all agents working in this repository.
These mandates apply **at all times** with **zero exceptions**.

---

## Core Mandates (Must ALWAYS Be Followed)

## 1. No mocking allowed, ever

- No mocks, stubs, fakes, or any test double.
- Tests must use real implementations or real in-memory components shared with production.

## 2. BRANCH WORKFLOW - MANDATORY FOR ALL DEVELOPMENT

**ABSOLUTE REQUIREMENT**: ALL development work MUST follow proper branch workflow

- **FORBIDDEN**: Direct commits to `main` branch (production releases only)
- **FORBIDDEN**: Direct commits to `develop` branch (integration only)
- **MANDATORY**: All work on feature branches off `develop`
- **MANDATORY**: Branch naming convention: `<type>/<description>` (feature/user-auth, fix/cli-sync, refactor/cleanup)
- **MANDATORY**: Read `docs/BRANCH_WORKFLOW.md` for complete workflow rules
- **MANDATORY**: Use `./dev_tools/git-helpers.sh start-branch` for branch creation
- **ENFORCED**: Build scripts validate branch compliance and refuse work on main/develop
- **ZERO EXCEPTIONS**: This applies to ALL agents at ALL times

## 3. PATH SECURITY
```

</details>
