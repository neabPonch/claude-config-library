---
name: pando85__kaniop__skill
source: https://github.com/pando85/kaniop/blob/4a8c85a08aeb191f00ee3309b42d8c19dfbe1e96/.opencode/skills/release/SKILL.md
repo: pando85/kaniop
kind: skill
stars: 106
last_pushed: 2026-06-15T06:48:49Z
license: agpl-3.0
score: 9
domains: [devops, rust, kubernetes, cli-tools]
tags: [release, semver, ci-cd, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# pando85/kaniop — skill

**Why it's worth keeping:** Demonstrates excellent patterns for high-stakes tasks by including 'Decision Guides' for logic, explicit 'Prerequisites' to prevent state errors, and a 'What NOT to Do' section for guardrails.

**Summary:** A highly rigorous release orchestration skill that combines pre-flight environmental checks, semantic version decision logic, and multi-step build propagation.

**Source credibility:** Strong; highly specific repository with 106 stars and active maintenance.

**Recency:** Current; utilizes modern toolchains like git-cliff and Cargo workspace patterns.

**Source:** [pando85/kaniop/.opencode/skills/release/SKILL.md](https://github.com/pando85/kaniop/blob/4a8c85a08aeb191f00ee3309b42d8c19dfbe1e96/.opencode/skills/release/SKILL.md) · 106★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release
description: Prepare and publish a new release. Use when the user asks to release, cut a release, or publish a new version.
---

## Purpose

Release a new version of Kaniop using the release script and CI pipeline.

## When to use

Use this skill when:
- The user asks to release a new version
- The user asks to cut a release or publish
- The user asks to tag a new version

## Prerequisites

Before releasing, verify:

1. **Working tree is clean** — no uncommitted changes
2. **You are on `master`** — releases only happen from master
3. **Local master is up to date with origin/master**
4. **No commits ahead of origin/master** (output of `git rev-list --count origin/master..HEAD` must be 0)
5. **Repository is not a shallow clone** — git-cliff needs full history for accurate changelogs

Check with:
```bash
git status --short
git rev-parse --abbrev-ref HEAD
git pull origin master
git rev-list --count origin/master..HEAD
git tag --sort=-creatordate | head -3
git log --oneline v<latest_tag>..HEAD
```

## Version Decision Guide

Use Semantic Versioning (MAJOR.MINOR.PATCH). Determine the bump type by analyzing commits since the last release.

### Major Version (X.0.0)

Bump
```

</details>
