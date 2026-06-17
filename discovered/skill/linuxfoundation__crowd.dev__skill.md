---
name: linuxfoundation__crowd.dev__skill
source: https://github.com/linuxfoundation/crowd.dev/blob/7cb7da7d78b590f69be8f6f1730b474710ea9d60/.claude/skills/dco/SKILL.md
repo: linuxfoundation/crowd.dev
kind: skill
stars: 3370
last_pushed: 2026-06-15T11:10:43Z
license: apache-2.0
score: 8
domains: [cli-tools, devops, git-workflow]
tags: [git, dco, sign-off, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# linuxfoundation/crowd.dev — skill

**Why it's worth keeping:** Includes a sophisticated verification command to validate signatures and emphasizes safer force-pushing practices like --force-with-lease.

**Summary:** A surgical guide for retroactively adding required DCO sign-offs to Git commit history via amend, rebase, or cherry-pick.

**Source credibility:** Highly credible; part of a major Linux Foundation project with high star count and recent activity.

**Recency:** Current; provides modern Git best practices compatible with contemporary workflows.

**Source:** [linuxfoundation/crowd.dev/.claude/skills/dco/SKILL.md](https://github.com/linuxfoundation/crowd.dev/blob/7cb7da7d78b590f69be8f6f1730b474710ea9d60/.claude/skills/dco/SKILL.md) · 3370★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dco
description: >
  Recover from missing DCO sign-off on commits. Handles the single-commit
  amend, older-commit recovery via interactive rebase or cherry-pick,
  and explains the Probot DCO check that blocks PRs without sign-off.
  Use when a PR fails the DCO check, when a commit needs a Signed-off-by
  trailer added retroactively, or when sign-off was forgotten during
  rebase / cherry-pick / amend.
allowed-tools: Bash, Read, Edit
---

# DCO Sign-off Recovery

All commits in this repo must carry a `Signed-off-by:` trailer (Developer Certificate of Origin). The Probot DCO check on PRs blocks merge until every commit is signed.

The standard way to add it is with `--signoff` at commit time. This skill handles the cases where that was missed.

## Case 1: Last commit only

```bash
git commit --amend --signoff -S --no-edit
git push --force-with-lease
```

`--force-with-lease` is preferred over plain `--force` — it refuses if someone else has pushed to the branch since you last fetched.

## Case 2: Older commit on the same branch

Find the commit hash of the oldest unsigned commit:

```bash
git log --pretty='%h %s %(trailers:key=Signed-off-by,valueonly)' origin/main..HEAD
#
```

</details>
