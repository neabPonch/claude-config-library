---
name: fagemx__gstack-game__skill-tmpl
source: https://github.com/fagemx/gstack-game/blob/7259ab9782fa9c17e45c16f1fb8347823ddb4379/skills/careful/SKILL.md.tmpl
repo: fagemx/gstack-game
kind: skill
stars: 38
last_pushed: 2026-05-31T15:29:42Z
license: mit
score: 8
domains: [cli-tools, security, devops]
tags: [safety, guardrails, bash, git]
curated: 2026-06-15
curated_by: config-scout
---

# fagemx/gstack-game — skill

**Why it's worth keeping:** Uses a highly structured pattern-to-risk mapping system and mandates a specific, high-visibility warning template for the agent to follow before execution.

**Summary:** Acts as a defensive wrapper that identifies and interrupts potentially destructive terminal commands to require explicit human confirmation.

**Source credibility:** Specialized repository with active maintenance and growing social proof via stars.

**Recency:** Extremely current; updated within the last month.

**Source:** [fagemx/gstack-game/skills/careful/SKILL.md.tmpl](https://github.com/fagemx/gstack-game/blob/7259ab9782fa9c17e45c16f1fb8347823ddb4379/skills/careful/SKILL.md.tmpl) · 38★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: careful
description: "Safety mode. Warns before destructive commands (rm -rf, DROP TABLE, git push -f, force delete). Does NOT restrict file editing scope — use /guard for that."
user_invocable: true
preamble-tier: 1
---
<!-- AUTO-GENERATED from SKILL.md.tmpl — do not edit directly -->
<!-- Regenerate: bun scripts/gen-skill-docs.ts -->

{{PREAMBLE}}

# /careful: Destructive Command Safety

Activates heightened awareness for destructive operations. When active, flag and confirm before executing any potentially destructive command.

## What triggers a warning

| Pattern | Risk | Action |
|---------|------|--------|
| `rm -rf` (except node_modules, .next, dist, build, __pycache__) | File deletion | Confirm before executing |
| `git push -f` / `git push --force` | History rewrite | Confirm + warn about remote impact |
| `git reset --hard` | Uncommitted work loss | Confirm + suggest stash first |
| `git clean -f` | Untracked file deletion | Confirm + list what will be deleted |
| `git branch -D` | Branch deletion | Confirm + check if merged |
| `DROP TABLE` / `DROP DATABASE` | Data destruction | Confirm + verify environment |
| `TRUNCATE` | Data deletion | Confirm |
| `docker
```

</details>
