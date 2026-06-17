---
name: sbusso__claudeclaw__skill
source: https://github.com/sbusso/claudeclaw/blob/1395af4ed2b9be6dd6dc35a3c6596d0eaa80d753/skills/update-claudeclaw/SKILL.md
repo: sbusso/claudeclaw
kind: skill
stars: 178
last_pushed: 2026-06-12T21:36:44Z
license: mit
score: 9
domains: [cli-tools, devops, git]
tags: [git-sync, fork-management, automation]
curated: 2026-06-15
curated_by: config-scout
---

# sbusso/claudeclaw — skill

**Why it's worth keeping:** It demonstrates excellent agentic patterns: preflight checks, dry-run conflict detection, low-token file access strategies, and automated breaking-change detection via CHANGELOG parsing.

**Summary:** A sophisticated Git workflow skill that automates upstream synchronization for customized forks using safety backups and categorized change previews.

**Source credibility:** High quality; part of an active project (ClaudeClaw) with clear engineering standards.

**Recency:** 

**Source:** [sbusso/claudeclaw/skills/update-claudeclaw/SKILL.md](https://github.com/sbusso/claudeclaw/blob/1395af4ed2b9be6dd6dc35a3c6596d0eaa80d753/skills/update-claudeclaw/SKILL.md) · 178★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: update-claudeclaw
description: Efficiently bring upstream ClaudeClaw updates into a customized install, with preview, selective cherry-pick, and low token usage.
---

# About

Your ClaudeClaw fork drifts from upstream as you customize it. This skill pulls upstream changes into your install without losing your modifications.

Run `/update-claudeclaw` in Claude Code.

## How it works

**Preflight**: checks for clean working tree (`git status --porcelain`). If `upstream` remote is missing, asks you for the URL (defaults to `https://github.com/sbusso/claudeclaw.git`) and adds it. Detects the upstream branch name (`main` or `master`).

**Backup**: creates a timestamped backup branch and tag (`backup/pre-update-<hash>-<timestamp>`, `pre-update-<hash>-<timestamp>`) before touching anything. Safe to run multiple times.

**Preview**: runs `git log` and `git diff` against the merge base to show upstream changes since your last sync. Groups changed files into categories:
- **Skills** (`.claude/skills/`): unlikely to conflict unless you edited an upstream skill
- **Source** (`src/`): may conflict if you modified the same files
- **Build/config** (`package.json`, `tsconfig*.json`, `ag
```

</details>
