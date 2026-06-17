---
name: shopsys__shopsys__skill
source: https://github.com/shopsys/shopsys/blob/08abae4689db562acbcc94cbebb22e49484d43f2/.agents/skills/commit/SKILL.md
repo: shopsys/shopsys
kind: skill
stars: 348
last_pushed: 2026-06-15T13:55:13Z
license: other
score: 9
domains: [cli-tools, devops, workflow-automation]
tags: [git, commit, workflow, productivity]
curated: 2026-06-16
curated_by: config-scout
---

# shopsys/shopsys — skill

**Why it's worth keeping:** The distinction between present vs. past tense for behavior vs. structure and specific rules for coupling lockfiles/tests are highly professional, transferable patterns.

**Summary:** An advanced git commit skill that enforces atomic, functional grouping and strict semantic message formatting.

**Source credibility:** High; sourced from a maintained, professional enterprise-grade platform repository.

**Recency:** Current; utilizes modern git workflow logic compatible with current agentic capabilities.

**Source:** [shopsys/shopsys/.agents/skills/commit/SKILL.md](https://github.com/shopsys/shopsys/blob/08abae4689db562acbcc94cbebb22e49484d43f2/.agents/skills/commit/SKILL.md) · 348★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: commit
description: >
  Commit Command — Analyzes uncommitted changes and creates logical, atomic, grouped commits
  following Shopsys commit guidelines. Use when the user asks to commit, create commits,
  or invokes /commit.
user_invocable: true
version: 1.0.0
---

# Commit Command

Analyzes uncommitted changes and creates logical, atomic, grouped commits following [Shopsys commit guidelines](https://docs.shopsys.com/en/18.0/contributing/guidelines-for-creating-commits/).

## Workflow

### Step 1: Gather Changes

```bash
git status                       # staged, unstaged, and untracked files
git diff --stat                  # unstaged changes summary
git diff                         # unstaged changes detail
git diff --cached --stat         # staged changes summary
git diff --cached                # staged changes detail
git diff --name-status           # detect renames, moves, deletions
git diff --cached --name-status  # same for staged
```

**Warning:** Skip sensitive files (`.env`, credentials, API keys) — warn user if detected.

### Step 2: Analyze and Group

Review all changes and group them into **atomic, functional units**:

- **By feature/functionality** — chang
```

</details>
