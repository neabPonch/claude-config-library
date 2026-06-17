---
name: lee-to__ai-factory__skill
source: https://github.com/lee-to/ai-factory/blob/920b99c1d1b6c1becce65ce3158df3553acdefb4/skills/aif-ci/SKILL.md
repo: lee-to/ai-factory
kind: skill
stars: 964
last_pushed: 2026-06-14T09:31:46Z
license: unknown
score: 9
domains: [devops, ci-cd, automation]
tags: [github-actions, gitlab-ci, pipeline, devops, project-analysis]
curated: 2026-06-15
curated_by: config-scout
---

# lee-to/ai-factory — skill

**Why it's worth keeping:** The logic uses a tiered mode system (generate/enhance/audit) and includes highly specific mappings for language versions and lock-file installation commands. It also introduces a valuable 'skill-context' pattern for overriding general instructions with project-specific rules.

**Summary:** A sophisticated CI/CD generator that performs deep project introspection to create production-ready GitHub Actions or GitLab pipelines.

**Source credibility:** High credibility; the repository has significant social proof with 964 stars.

**Recency:** Current; utilizes modern tool-calling patterns and contemporary developer workflows.

**Source:** [lee-to/ai-factory/skills/aif-ci/SKILL.md](https://github.com/lee-to/ai-factory/blob/920b99c1d1b6c1becce65ce3158df3553acdefb4/skills/aif-ci/SKILL.md) · 964★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aif-ci
description: Generate CI/CD pipeline (GitHub Actions / GitLab CI) with linting, static analysis, tests, security. Use when user says "ci", "setup ci", "github actions", "gitlab ci", "pipeline".
argument-hint: "[github|gitlab] [--enhance]"
allowed-tools: Read Edit Glob Grep Write Bash(git *) AskUserQuestion Questions
disable-model-invocation: true
metadata:
  author: AI Factory
  version: "1.0"
  category: ci
---

# CI — Pipeline Configuration Generator

Analyze a project and generate production-grade CI/CD pipeline configuration for GitHub Actions or GitLab CI. Generates separate jobs for linting, static analysis, tests, and security scanning — adapted to the project's language, framework, and existing tooling.

**Three modes based on what exists:**

| What exists | Mode | Action |
|-------------|------|--------|
| No CI config | `generate` | Create pipeline from scratch with interactive setup |
| CI config exists but incomplete | `enhance` | Audit & improve, add missing jobs |
| Full CI config | `audit` | Audit against best practices, fix gaps |

---

## Step 0: Load Project Context

Read the project description if available:

```
Read .ai-factory/DESCRIPTION.md
`
```

</details>
