---
name: Getty__karr__claude-skill
source: https://github.com/Getty/karr/blob/5beb1a8f32a5a9a8f5fa6d2ddc5c382d72b77c92/share/claude-skill.md
repo: Getty/karr
kind: skill
stars: 6
last_pushed: 2026-06-05T02:36:32Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, workflow-automation]
tags: [kanban, git-native, multi-agent, task-management]
curated: 2026-06-17
curated_by: config-scout
---

# Getty/karr — skill

**Why it's worth keeping:** The use of `refs/karr/*` to store task data keeps the workspace clean; its 'claim' and 'pick' logic is a perfect pattern for preventing race conditions and duplicate work among multiple agents.

**Summary:** A Git-native Kanban system that uses Git refs to manage task state and multi-agent coordination without polluting the working directory. It provides robust mechanisms for claiming, handoff, and status tracking in distributed agent workflows.

**Source credibility:** Low star count, but the implementation details suggest highly sophisticated Git-internal knowledge.

**Recency:** Highly current; explicitly includes support for `claude-code` skills.

**Source:** [Getty/karr/share/claude-skill.md](https://github.com/Getty/karr/blob/5beb1a8f32a5a9a8f5fa6d2ddc5c382d72b77c92/share/claude-skill.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: karr
description: Use when managing Git-native kanban tasks or shared helper refs with the karr CLI in agent workflows.
---

# karr — Kanban Assignment & Responsibility Registry

Git-native kanban board for multi-agent workflows. Canonical board state lives in
`refs/karr/*`, not in a checked-in `karr/` directory. Commands materialize a
temporary task/config view only while they run.

## Commands

### Initialize

```bash
karr init [--name NAME] [--statuses s1,s2,s3] [--claude-skill]
```

Creates the board refs inside the current Git repository. With
`--claude-skill`, installs this skill to `.claude/skills/karr/SKILL.md`.

### Create task

```bash
karr create "Title" [--status STATUS] [--priority PRIORITY] [--tags t1,t2] [--body TEXT]
karr create --title "Title" --assignee NAME --due 2026-03-15
```

### List tasks

```bash
karr list                                    # all non-archived
karr list --status todo,in-progress          # filter by status
karr list --priority high,critical           # filter by priority
karr list --tag backend                      # filter by tag
karr list -s "search term"                   # search title/body/tags
karr list --sort priority --reve
```

</details>
