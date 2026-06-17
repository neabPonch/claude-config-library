---
name: neurosie__streetsweeper
source: https://github.com/neurosie/streetsweeper/blob/72f41e5e009bb8efa58413155f735ba06337ea03/Claude.md
repo: neurosie/streetsweeper
kind: claude-md
stars: 1
last_pushed: 2026-05-21T20:57:15Z
license: unknown
score: 9
domains: [web-frontend, fullstack, devops]
tags: [workflow-management, session-handoff, git-hooks, t3-stack]
curated: 2026-06-15
curated_by: config-scout
---

# neurosie/streetsweeper — claude-md

**Why it's worth keeping:** The mandatory end-of-session checklist (pushing/syncing) and explicit instructions for Git hook installation are elite, transferable patterns for preventing lost progress.

**Summary:** Defines a strict 'Landing the Plane' protocol to ensure all work is pushed and issue statuses are updated before a session ends.

**Source credibility:** Low star count, but the highly structured workflow suggests high-discipline authorship.

**Recency:** Current; uses modern tech stacks and specifically optimizes for AI assistant context.

**Source:** [neurosie/streetsweeper/Claude.md](https://github.com/neurosie/streetsweeper/blob/72f41e5e009bb8efa58413155f735ba06337ea03/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# StreetSweeper

## Project Overview

StreetSweeper is a local geography guessing game where users pick a town or city and try to name as many streets as they can - like Sporcle for your neighborhood.

**Live Site**: https://streetsweeper.fly.dev/

## Issue tracking

This project uses **bd** (beads) for issue tracking. Run `bd onboard` to get started.

### Quick Reference

```bash
bd ready              # Find available work
bd show <id>          # View issue details
bd update <id> --status in_progress  # Claim work
bd close <id>         # Complete work
bd sync               # Sync with git
```

### Landing the Plane (Session Completion)

**When ending a work session**, you MUST complete ALL steps below. Work is NOT complete until `git push` succeeds.

**MANDATORY WORKFLOW:**

1. **File issues for remaining work** - Create issues for anything that needs follow-up
2. **Run quality gates** (if code changed) - Tests, linters, builds
3. **Update issue status** - Close finished work, update in-progress items
4. **PUSH TO REMOTE** - This is MANDATORY:
   ```bash
   git pull --rebase
   bd sync
   git push
   git status  # MUST show "up to date with origin"
   ```
5. **Clean up** - Clear s
```

</details>
