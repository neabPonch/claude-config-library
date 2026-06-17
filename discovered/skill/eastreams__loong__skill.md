---
name: eastreams__loong__skill
source: https://github.com/eastreams/loong/blob/0e862d294c5e4f65444d99bf7b44db4e4695bf6c/crates/app/skills/github-issues/SKILL.md
repo: eastreams/loong
kind: skill
stars: 641
last_pushed: 2026-06-15T14:25:54Z
license: mit
score: 8
domains: [cli-tools, project-management, devops]
tags: [github, issue-tracking, automation]
curated: 2026-06-15
curated_by: config-scout
---

# eastreams/loong — skill

**Why it's worth keeping:** The setup logic automatically extracts repo metadata from git remotes and provides robust fallback mechanisms (curl + python) if the gh CLI is unavailable or unauthenticated.

**Summary:** Provides a dual-track workflow for managing GitHub issues using both the 'gh' CLI and raw REST API via curl.

**Source credibility:** High; part of a popular, actively maintained repository with significant community interest.

**Recency:** Current; uses modern GitHub API patterns and standard CLI tools.

**Source:** [eastreams/loong/crates/app/skills/github-issues/SKILL.md](https://github.com/eastreams/loong/blob/0e862d294c5e4f65444d99bf7b44db4e4695bf6c/crates/app/skills/github-issues/SKILL.md) · 641★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: github-issues
description: Create, manage, triage, and close GitHub issues. Search existing issues, add labels, assign people, and link to PRs. Works with gh CLI or falls back to git + GitHub REST API via curl.
version: 1.1.0
author: Hermes Agent
license: MIT
metadata:
  hermes:
    tags: [GitHub, Issues, Project-Management, Bug-Tracking, Triage]
    related_skills: [github-auth, github-pr-workflow]
---

# GitHub Issues Management

Create, search, triage, and manage GitHub issues. Each section shows `gh` first, then the `curl` fallback.

## Prerequisites

- Authenticated with GitHub (see `github-auth` skill)
- Inside a git repo with a GitHub remote, or specify the repo explicitly

### Setup

```bash
if command -v gh &>/dev/null && gh auth status &>/dev/null; then
  AUTH="gh"
else
  AUTH="git"
  if [ -z "$GITHUB_TOKEN" ]; then
    if [ -f ~/.hermes/.env ] && grep -q "^GITHUB_TOKEN=" ~/.hermes/.env; then
      GITHUB_TOKEN=$(grep "^GITHUB_TOKEN=" ~/.hermes/.env | head -1 | cut -d= -f2 | tr -d '\n\r')
    elif grep -q "github.com" ~/.git-credentials 2>/dev/null; then
      GITHUB_TOKEN=$(grep "github.com" ~/.git-credentials 2>/dev/null | head -1 | sed 's|https://[^:]*:\([^@]
```

</details>
