---
name: GoogleCloudPlatform__spring-cloud-gcp__skill
source: https://github.com/GoogleCloudPlatform/spring-cloud-gcp/blob/723a06e9c9e173773638fd048b7137bba2c51b0d/.agents/skills/backport/SKILL.md
repo: GoogleCloudPlatform/spring-cloud-gcp
kind: skill
stars: 544
last_pushed: 2026-06-15T04:31:24Z
license: apache-2.0
score: 9
domains: [devops, git-workflows, maintenance]
tags: [backporting, github-cli, git]
curated: 2026-06-15
curated_by: config-scout
---

# GoogleCloudPlatform/spring-cloud-gcp — skill

**Why it's worth keeping:** Uses extremely strict naming conventions and exact command-line templates that eliminate agent ambiguity; provides deterministic metadata rules (title/body) required for automated workflows.

**Summary:** A rigorous SOP for backporting pull requests from a main branch to active release branches using Git and GitHub CLI.

**Source credibility:** High: Official Google Cloud Platform repository with high star count and recent activity.

**Recency:** Current: Uses modern GitHub CLI (gh) patterns consistent with modern developer workflows.

**Source:** [GoogleCloudPlatform/spring-cloud-gcp/.agents/skills/backport/SKILL.md](https://github.com/GoogleCloudPlatform/spring-cloud-gcp/blob/723a06e9c9e173773638fd048b7137bba2c51b0d/.agents/skills/backport/SKILL.md) · 544★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: backport
description: >-
  Backports pull requests that have been merged into the main branch across to older
  active release branches (e.g., 6.x, 7.x). Use when instructed to cherry-pick, backport,
  or migrate merged pull requests or commits to older support branches in the repository.
---

# Backporting Pull Requests

This document defines the standard operating procedures and conventions for AI agents performing backporting tasks in the `spring-cloud-gcp` repository.

## Prerequisites
- Access to the `git` command line tool.
- Access to the GitHub CLI (`gh`), authenticated with sufficient repository scopes to create branches and pull requests.

## Branching & Naming Conventions
- **Target Release Branches:** Active support branches such as `6.x` and `7.x`.
- **Local/Head Branch Name:** `<target-branch>-cherry-pick-<short-commit-hash>`
  - *Example:* `6.x-cherry-pick-366c6fe` (where `366c6fe` is the 7-character short hash of the commit from `main`).

## Pull Request Metadata Conventions
To ensure consistency and traceability across releases, backport pull requests MUST adhere to the following formatting rules:
- **PR Base:** The target release branch (e.g., `6.x`).
-
```

</details>
