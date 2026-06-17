---
name: rohitg00__pro-workflow__skill
source: https://github.com/rohitg00/pro-workflow/blob/5c313e2c7f4cbb27f6cf7b97e7d2928a26963918/skills/sprint-status/SKILL.md
repo: rohitg00/pro-workflow
kind: skill
stars: 2302
last_pushed: 2026-06-08T20:24:42Z
license: unknown
score: 8
domains: [cli-tools, workflows, agents-ai]
tags: [parallel-work, status-reporting, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# rohitg00/pro-workflow — skill

**Why it's worth keeping:** Uses specific state-based reporting (BLOCKED, NEEDS_INFO) and mandates 'sensible defaults' for decisions to minimize user cognitive load.

**Summary:** Standardizes communication via structured status headers to prevent context mismatch when running multiple Claude Code sessions simultaneously.

**Source credibility:** High; the source repository is highly starred and actively maintained.

**Recency:** Current; utilizes modern CLI/Git workflows like worktrees and process detection.

**Source:** [rohitg00/pro-workflow/skills/sprint-status/SKILL.md](https://github.com/rohitg00/pro-workflow/blob/5c313e2c7f4cbb27f6cf7b97e7d2928a26963918/skills/sprint-status/SKILL.md) · 2302★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sprint-status
description: Track parallel work sessions and prevent confusion across multiple Claude Code instances. Every major step ends with a status line. Every question re-states project, branch, and task.
---

# Sprint Status

When running multiple Claude Code sessions in parallel, confusion is the enemy. This skill ensures every session identifies itself and every step reports its state.

## Session Identification

Every response that involves a decision, plan, or significant action starts with orientation:

```text
SESSION: my-app | branch: feat/auth | task: Add JWT refresh tokens
```

This takes one line. It costs almost nothing. It prevents the user from applying feedback to the wrong session.

### Detecting Parallel Sessions

Check for sibling Claude Code processes:

```bash
pgrep -af "claude" | grep -v "$$" | head -5
```

Or check for active worktrees:

```bash
git worktree list 2>/dev/null
```

Or look for session markers (written by session-start.js / session-end.js):

```bash
ls $TMPDIR/pro-workflow/sessions/ 2>/dev/null | tail -5
```

If multiple sessions are detected, always include the session identification header. If only one session is running, includ
```

</details>
