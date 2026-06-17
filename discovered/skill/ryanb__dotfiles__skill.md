---
name: ryanb__dotfiles__skill
source: https://github.com/ryanb/dotfiles/blob/74946de1e1c52e479047672dca4230bb83505f12/claude/skills/bisect/SKILL.md
repo: ryanb/dotfiles
kind: skill
stars: 2387
last_pushed: 2026-06-12T21:10:21Z
license: mit
score: 8
domains: [cli-tools, devops]
tags: [git, debugging, automation]
curated: 2026-06-15
curated_by: config-scout
---

# ryanb/dotfiles — skill

**Why it's worth keeping:** It includes a proactive step to jump backwards in chunks to establish a 'good' baseline and enforces strict pre-flight checks for a clean working tree.

**Summary:** Automates a full git bisect workflow by providing a heuristic to find a known-good commit before initiating formal binary search.

**Source credibility:** High; part of a highly-starred (2k+) developer dotfiles repository.

**Recency:** Current; uses standard git commands compatible with modern CLI environments.

**Source:** [ryanb/dotfiles/claude/skills/bisect/SKILL.md](https://github.com/ryanb/dotfiles/blob/74946de1e1c52e479047672dca4230bb83505f12/claude/skills/bisect/SKILL.md) · 2387★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bisect
description: Git bisect to find the first bad commit by running a test command.
user-invocable-only: true
allowed-tools: Bash, Read, Glob, Grep, AskUserQuestion
argument-hint: <instructions on what command to run to test each commit>
---

# bisect — Find the First Bad Commit

Use `git bisect` to binary-search through commit history and find the first commit that introduced a failure.

## Step 1: Ensure clean working tree

Check that there are no staged or unstaged changes. If there are, **stop and tell the user** they need a clean working tree before bisecting, since git bisect checks out older commits.

```bash
git status --porcelain
```

If the output is non-empty, stop and ask the user to commit or stash their changes first.

## Step 2: Determine the test command

Use `$ARGUMENTS` to understand what the user wants to test. This should describe a command or check that fails on the current commit. Determine the exact shell command to run.

## Step 3: Verify the current commit is bad

Run the test command on the current commit (HEAD). If it **passes** (exits 0), stop and tell the user — the current commit doesn't exhibit the failure, so there's nothing to bisect.
```

</details>
