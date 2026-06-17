---
name: teambit__bit__skill
source: https://github.com/teambit/bit/blob/1b166c5ace337cc978b47d10594d2d631f68272b/.claude/skills/generate-release-notes/SKILL.md
repo: teambit/bit
kind: skill
stars: 18408
last_pushed: 2026-06-12T17:26:15Z
license: other
score: 9
domains: [cli-tools, devops, documentation]
tags: [release-notes, git-automation, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# teambit/bit — skill

**Why it's worth keeping:** It utilizes an 'intermediate files' pattern (raw vs filtered) so users can audit the agent's logic; it also provides explicit filtering rules and enrichment steps using PR metadata.

**Summary:** A highly structured workflow for generating categorized release notes by fetching and enriching git commit data via the GitHub CLI.

**Source credibility:** Very high, sourced from a major open-source repository with 18k+ stars.

**Recency:** Current; relies on modern GitHub CLI (`gh`) patterns common in modern dev workflows.

**Source:** [teambit/bit/.claude/skills/generate-release-notes/SKILL.md](https://github.com/teambit/bit/blob/1b166c5ace337cc978b47d10594d2d631f68272b/.claude/skills/generate-release-notes/SKILL.md) · 18408★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: generate-release-notes
description: Generate comprehensive release notes for Bit from git commits and pull requests. Use when creating release notes, building changelogs, documenting version releases, or preparing a new Bit release.
---

# Generate Release Notes for Bit

This skill helps generate release notes for Bit following the established patterns and guidelines.

## Important: Intermediate Files

All intermediate steps must be saved to `releases-docs/temp-files/` for review. This folder is gitignored.

**Required intermediate files:**

1. `raw-commits.md` - Raw commit data from GitHub API
2. `filtered-commits.md` - Two sections: filtered out commits and kept commits

## Workflow

Follow these steps to generate release notes:

### Step 1: Setup Temp Directory

First, ensure the temp directory exists:

```bash
mkdir -p releases-docs/temp-files
```

### Step 2: Determine the Commit Range

1. **Get the latest release tag and commit:**

   ```bash
   # Get latest release tag
   gh release view --repo teambit/bit --json tagName -q '.tagName'

   # Get the commit SHA for the tag (handles annotated tags)
   TAG="v1.12.158"  # Replace with actual tag
   TAG_REF=$(gh api "rep
```

</details>
