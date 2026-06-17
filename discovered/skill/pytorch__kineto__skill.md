---
name: pytorch__kineto__skill
source: https://github.com/pytorch/kineto/blob/1d43601b8e77135a0fd3b99125de48972a2ff11c/.claude/skills/kineto-release/SKILL.md
repo: pytorch/kineto
kind: skill
stars: 960
last_pushed: 2026-06-13T12:59:28Z
license: other
score: 8
domains: [devops, git-workflows, cli-tools]
tags: [submodule, dependency-management, automation]
curated: 2026-06-15
curated_by: config-scout
---

# pytorch/kineto — skill

**Why it's worth keeping:** Demonstrates high-quality pattern for cross-repository state management and using git history to auto-generate changelog entries within commit messages.

**Summary:** Automates the synchronization of a git submodule by updating its pointer in a parent repository and generating a detailed commit message containing the delta's history.

**Source credibility:** High; sourced from a highly-starred, active performance profiling library used in PyTorch.

**Recency:** Current; uses modern Claude Code tool specifications and argument hints.

**Source:** [pytorch/kineto/.claude/skills/kineto-release/SKILL.md](https://github.com/pytorch/kineto/blob/1d43601b8e77135a0fd3b99125de48972a2ff11c/.claude/skills/kineto-release/SKILL.md) · 960★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kineto-release
description: Update the third_party/kineto submodule in PyTorch to the latest commit from this kineto repo and commit the change. Use when updating the kineto submodule hash for a release.
disable-model-invocation: true
argument-hint: "[commit-hash]"
allowed-tools: Bash(git:*), Read, AskUserQuestion
---

# Update Kineto Submodule

Update the `third_party/kineto` submodule in a local PyTorch repo to point to a
commit from this Kineto repo.

If a commit hash is provided via `$ARGUMENTS`, use that as the target hash.
Otherwise, use the tip of main from this repo.

## Prerequisites

Before starting, you need the path to the local PyTorch repo. If you do not
already know it from prior conversation context, ask the user:

> "What is the path to your local PyTorch repo?"

The PyTorch repo is required — do not proceed without it. Store the path as
`$PYTORCH` for the steps below.

## Steps

1. **(PyTorch) Get the current submodule hash:**
   ```
   cd $PYTORCH && git submodule status third_party/kineto | awk '{print $1}' | sed 's/^[-+]//'
   ```

2. **(Kineto) Get the target hash.** If `$ARGUMENTS` is provided, use it. Otherwise, get
   the tip of main from this rep
```

</details>
