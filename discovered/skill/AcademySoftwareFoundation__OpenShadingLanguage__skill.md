---
name: AcademySoftwareFoundation__OpenShadingLanguage__skill
source: https://github.com/AcademySoftwareFoundation/OpenShadingLanguage/blob/b7fff57a2a14b5471a926b7cdb84c238b3ba82e9/.agents/skills/release-notes-update/SKILL.md
repo: AcademySoftwareFoundation/OpenShadingLanguage
kind: skill
stars: 2301
last_pushed: 2026-06-15T17:56:27Z
license: bsd-3-clause
score: 9
domains: [devops, cli-tools, version-control]
tags: [release-notes, git, automation]
curated: 2026-06-16
curated_by: config-scout
---

# AcademySoftwareFoundation/OpenShadingLanguage — skill

**Why it's worth keeping:** Demonstrates how to structure multi-step workflows involving tool execution, file reading/writing, and complex conditional logic for cross-branch synchronization.

**Summary:** Automates high-precision release note generation using git-cliff with strict formatting rules for different release tiers.

**Source credibility:** High; comes from a mature, industry-standard graphics project (OpenShadingLanguage).

**Recency:** Current; utilizes modern Git/CLI orchestration techniques compatible with Claude Code.

**Source:** [AcademySoftwareFoundation/OpenShadingLanguage/.agents/skills/release-notes-update/SKILL.md](https://github.com/AcademySoftwareFoundation/OpenShadingLanguage/blob/b7fff57a2a14b5471a926b7cdb84c238b3ba82e9/.agents/skills/release-notes-update/SKILL.md) · 2301★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-notes-update
description: Generate or update release notes for a patch, minor, or major release, or just to update main. Run git-cliff, organize and edit the output per project conventions, and insert into CHANGES.md.
argument-hint: [patch|minor|major|main] [prev-tag]
---

Generate release notes for an OSL release.

Arguments: `$ARGUMENTS`
- First argument (optional): release type — `patch` (default), `minor`, `major`, or `main`.
- Second argument (optional): previous release tag (e.g. `v3.1.2.0`). If omitted, find the most recent tag automatically. If the release type is `main`, instead of a tag, look for the last commit at which the CHANGES.md file was updated.

## Steps

1. **Determine the previous tag** if not provided:
   ```
   git describe --tags --abbrev=0
   ```
   or look at recent tags: `git tag --sort=-version:refname | head -10`.
   However, if the "release type" is `main`, instead of a tag, just find
   the commit at which CHANGES.md was last updated.

2. **Run git-cliff** to get raw commit data:
   ```
   git cliff -c src/doc/cliff.toml <prev-tag>..HEAD > /tmp/cliff-out.md
   ```
   Read `/tmp/cliff-out.md` to see the raw output.

3. **Read CHANGES.
```

</details>
