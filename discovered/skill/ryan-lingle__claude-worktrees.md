---
name: ryan-lingle__claude-worktrees
source: https://github.com/ryan-lingle/claude-worktrees/blob/460cdeb2edb643593f79941bb403e6fdb4f8d5c2/skill.md
repo: ryan-lingle/claude-worktrees
kind: skill
stars: 0
last_pushed: 2026-03-19T16:03:06Z
license: mit
score: 8
domains: [cli-tools, devops, git]
tags: [git-worktree, parallel-development, environment-isolation]
curated: 2026-06-15
curated_by: config-scout
---

# ryan-lingle/claude-worktrees — skill

**Why it's worth keeping:** It enforces a critical 'absolute path' rule for all file operations and provides a robust pattern for resource isolation (ports/databases) in multi-session workflows.

**Summary:** This skill manages Git worktrees with an automated port allocation system to enable parallel, isolated local development sessions.

**Source credibility:** Low star count and recent activity, but the high degree of technical specificity suggests an expert-level developer tool.

**Recency:** Very current; addresses fundamental friction points in Claude Code's multi-workspace capabilities.

**Source:** [ryan-lingle/claude-worktrees/skill.md](https://github.com/ryan-lingle/claude-worktrees/blob/460cdeb2edb643593f79941bb403e6fdb4f8d5c2/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: worktree
description: Manage git worktrees for parallel Claude Code sessions. Create, list, navigate, and remove worktrees with automatic port allocation for local native development.
allowed-tools: Bash, Read, Write, Edit, Glob, Grep
version: 1.3.0
---

# Git Worktree Skill

Manage git worktrees for running parallel Claude Code sessions on the same repository. Each worktree gets its own isolated file state while sharing git history. All development runs natively — no Docker.

## CRITICAL: Always Use Absolute Paths

**All file operations and commands MUST use absolute paths to the target worktree.** This allows working on any worktree from any session, regardless of the current working directory.

### Rules

1. **File tools** (Read, Edit, Write, Glob, Grep): Always use the full absolute path (e.g., `$HOME/worktrees/myapp-feature-auth/app/models/user.rb`)
2. **Git commands**: Use `git -C <worktree-path>` instead of relying on cwd (e.g., `git -C $HOME/worktrees/myapp-feature-auth status`)
3. **Tests**: Pass the absolute path to your test runner (e.g., `~/.claude/scripts/native-test $HOME/worktrees/myapp-feature-auth/test/models/user_test.rb`)
4. **Bundle/Rails**: Use `bash
```

</details>
