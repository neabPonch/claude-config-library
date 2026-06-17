---
name: benekuehn__socle__skill
source: https://github.com/benekuehn/socle/blob/26ae84b77434a1b2caf9942035943be7acaf84f0/cli/skills/socle-cli/SKILL.md
repo: benekuehn/socle
kind: skill
stars: 4
last_pushed: 2026-05-13T00:54:30Z
license: mit
score: 8
domains: [cli-tools, git-workflows, devops]
tags: [git, stacked-branches, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# benekuehn/socle — skill

**Why it's worth keeping:** It includes critical low-level details like metadata storage locations in .git/config and specific troubleshooting steps for resolving rebase conflicts.

**Summary:** This skill provides comprehensive command mappings and workflow guidance for the socle CLI to manage stacked Git branches.

**Source credibility:** A specialized niche tool with recent maintenance activity.

**Recency:** Highly current, pushed within the last month.

**Source:** [benekuehn/socle/cli/skills/socle-cli/SKILL.md](https://github.com/benekuehn/socle/blob/26ae84b77434a1b2caf9942035943be7acaf84f0/cli/skills/socle-cli/SKILL.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: socle-cli
description: Use this skill when you need to guide or automate usage of the socle CLI (the `so` command) for stacked-branch workflows, including installing `so`, tracking branch stacks, navigating up/down/top/bottom, creating stacked branches, restacking, syncing, or submitting stacked PRs.
---

# Socle CLI

## Overview
Enable consistent, step-by-step guidance for using the `so` CLI to manage stacked Git branches and pull requests.

## Quick start
- Install `so` with Homebrew (`brew install benekuehn/tap/socle`).
- Verify installation with `so --version`.
- Work inside a Git repository before running stack commands.

## Core tasks

### Create and track a stack
- Create a new stacked branch from the current branch with `so create <branch-name>`.
- If there are uncommitted changes, pass `-m "commit message"` to include them on the new branch.
- Set stack relationships by running `so track` on each branch in order from the base branch upward.

### Navigate the stack
- Move one branch up or down: `so up`, `so down`.
- Jump to the base-adjacent or top branch: `so bottom`, `so top`.
- Review the current stack and rebase status: `so log`.

### Update a stack
- Rebase t
```

</details>
