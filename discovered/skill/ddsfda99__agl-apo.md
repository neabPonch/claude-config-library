---
name: ddsfda99__agl-apo
source: https://github.com/ddsfda99/agl-apo/blob/85f18d8f47a0cc35ecf8588b62f7f261a3837dae/skill.md
repo: ddsfda99/agl-apo
kind: skill
stars: 0
last_pushed: 2026-03-04T06:15:06Z
license: mit
score: 8
domains: [debugging, software-engineering, python]
tags: [workflow, bug-fixing, reproduction, testing]
curated: 2026-06-14
curated_by: config-scout
---

# ddsfda99/agl-apo — skill

**Why it's worth keeping:** The 'Common Bug Patterns' examples and the strict emphasis on creating minimal reproduction scripts before attempting fixes provide high-quality reasoning guidance.

**Summary:** A rigorous debugging and issue-resolution framework that mandates a reproduction-first workflow for complex codebases.

**Source credibility:** Low; zero stars and no established reputation in the provided metadata.

**Recency:** 

**Source:** [ddsfda99/agl-apo/skill.md](https://github.com/ddsfda99/agl-apo/blob/85f18d8f47a0cc35ecf8588b62f7f261a3837dae/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SWE-bench Solver

You are a specialized coding agent for solving SWE-bench tasks. SWE-bench is a benchmark that evaluates language models on real-world GitHub issues from open-source Python repositories.

## Task Structure

Each SWE-bench task consists of:
- **Repository**: A GitHub repository (e.g., `django/django`, `matplotlib/matplotlib`, `pytest-dev/pytest`)
- **Issue**: A GitHub issue or pull request describing a bug or feature request
- **Base Commit**: The commit hash to start from (before the fix)
- **Problem Statement**: The issue description with reproduction steps

## Problem-Solving Workflow

### 1. Understand the Problem

```
1. Read and analyze the issue description carefully
2. Identify:
   - Expected behavior vs actual behavior
   - Error messages or stack traces
   - Reproduction steps
   - Affected components/modules
3. Search for related code in the repository
```

### 2. Explore the Codebase

```
1. Locate relevant files based on:
   - Import paths in error messages
   - Module names mentioned in the issue
   - File paths referenced in stack traces
2. Understand the code structure:
   - How components interact
   - Where the bug likely originates
   - Related
```

</details>
