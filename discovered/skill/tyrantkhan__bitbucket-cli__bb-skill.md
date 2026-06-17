---
name: tyrantkhan__bitbucket-cli__bb-skill
source: https://github.com/tyrantkhan/bitbucket-cli/blob/3aee4ecfca2c63dace66187936bf14e43ac3bfc4/docs/bb-skill.md
repo: tyrantkhan/bitbucket-cli
kind: skill
stars: 2
last_pushed: 2026-04-10T15:36:01Z
license: mit
score: 8
domains: [cli-tools, devops]
tags: [bitbucket, git-workflow, pr-review, devops]
curated: 2026-06-15
curated_by: config-scout
---

# tyrantkhan/bitbucket-cli — skill

**Why it's worth keeping:** The 'PR review workflow' is excellent; it provides a multi-step logic chain including how to handle different comment types and context gathering.

**Summary:** A high-density guide for the Bitbucket `bb` CLI that includes structured operational workflows.

**Source credibility:** Specific utility tool with high-quality, manually authored documentation patterns.

**Recency:** Current; uses modern CLI patterns like auto-detection of workspace/repo.

**Source:** [tyrantkhan/bitbucket-cli/docs/bb-skill.md](https://github.com/tyrantkhan/bitbucket-cli/blob/3aee4ecfca2c63dace66187936bf14e43ac3bfc4/docs/bb-skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bb
version: 1.2.0
description: Use the bb CLI to interact with Bitbucket Cloud — manage PRs, repos, and pipelines. Use when the user asks about Bitbucket pull requests, repositories, pipelines, or wants to perform Bitbucket operations.
allowed-tools: Bash(bb *)
---

You have access to `bb`, a CLI for Bitbucket Cloud. Use it via the Bash tool to help the user with Bitbucket operations.

bb auto-detects workspace and repo from git remotes, so most commands work without flags when inside a Bitbucket-hosted repo.

## Quick examples

### Pull requests

```sh
bb pr status                          # PRs for current branch, authored by you, requesting your review
bb pr list                            # list open PRs
bb pr view 42 --comments              # view PR with threaded comments
bb pr create --title "Add X" --destination main
bb pr diff 42                         # view diff
bb pr approve 42                      # approve
bb pr comment 42 --body "LGTM"        # add comment
bb pr comment 42 --body "Fix this" --file src/handler.go --line 55  # inline comment
bb pr comment 42 --body "Good point" --parent 764369882            # threaded reply
bb pr merge 42 --strategy squash
```

</details>
