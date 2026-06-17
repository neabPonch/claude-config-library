---
name: CherryHQ__cherry-studio__skill
source: https://github.com/CherryHQ/cherry-studio/blob/335e72e8446f461822de6206830f23b142f327d2/.agents/skills/prepare-release/SKILL.md
repo: CherryHQ/cherry-studio
kind: skill
stars: 47375
last_pushed: 2026-06-15T16:35:45Z
license: agpl-3.0
score: 9
domains: [devops, cli-tools, automation]
tags: [release-management, git-workflow, bilingual]
curated: 2026-06-15
curated_by: config-scout
---

# CherryHQ/cherry-studio — skill

**Why it's worth keeping:** Excellent use of 'user-focused' negative constraints to filter technical debt from public notes and provides a highly structured extraction logic for commit bodies.

**Summary:** Automates end-to-end release workflows including semver bumping, bilingual note generation from git logs, and PR creation.

**Source credibility:** High; the source is a major AI productivity project with significant star count and active maintenance.

**Recency:** Current; demonstrates advanced agentic patterns like cross-skill tool invocation and complex workflow orchestration.

**Source:** [CherryHQ/cherry-studio/.agents/skills/prepare-release/SKILL.md](https://github.com/CherryHQ/cherry-studio/blob/335e72e8446f461822de6206830f23b142f327d2/.agents/skills/prepare-release/SKILL.md) · 47375★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prepare-release
description: Prepare a new release by collecting commits, generating bilingual release notes, updating version files, and creating a release branch with PR. Use when asked to prepare/create a release, bump version, or run `/prepare-release`.
---

# Prepare Release

Automate the Cherry Studio release workflow: collect changes → generate bilingual release notes → update files → create release branch + PR → trigger CI/CD.

## Arguments

Parse the version intent from the user's message. Accept any of these forms:
- Bump type keyword: `patch`, `minor`, `major`
- Exact version: `x.y.z` or `x.y.z-pre.N` (e.g. `1.8.0`, `1.8.0-beta.1`, `1.8.0-rc.1`)
- Natural language: "prepare a beta release", "bump to 1.8.0-rc.2", etc.

Defaults to `patch` if no version is specified. Always echo the resolved target version back to the user before proceeding with any file edits.

- `--dry-run`: Preview only, do not create branch or PR.

## Workflow

### Step 1: Determine Version

1. Get the latest tag:
   ```bash
   git describe --tags --abbrev=0
   ```
2. Read current version from `package.json`.
3. Compute the new version based on the argument:
   - `patch` / `minor` / `major`:
```

</details>
