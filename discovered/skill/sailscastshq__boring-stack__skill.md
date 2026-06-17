---
name: sailscastshq__boring-stack__skill
source: https://github.com/sailscastshq/boring-stack/blob/2ebcf8b272c506a5e132dfa2ca7cc37ac2cb3c96/skills/quest/SKILL.md
repo: sailscastshq/boring-stack
kind: skill
stars: 499
last_pushed: 2026-05-28T11:31:53Z
license: mit
score: 8
domains: [backend, job-scheduling, sailsjs]
tags: [background-jobs, sails-js, cron]
curated: 2026-06-15
curated_by: config-scout
---

# sailscastshq/boring-stack — skill

**Why it's worth keeping:** Uses an excellent hierarchical pattern that directs the agent to specific rule files (rules/*.md) rather than overwhelming it with a single large context file.

**Summary:** Provides a structured entry point and documentation map for the Quest background job scheduling system within Sails.js.

**Source credibility:** High; part of the popular 'boring-stack' repository with significant GitHub stars and recent activity.

**Recency:** Current; follows modern modular documentation patterns ideal for LLM agent toolsets.

**Source:** [sailscastshq/boring-stack/skills/quest/SKILL.md](https://github.com/sailscastshq/boring-stack/blob/2ebcf8b272c506a5e132dfa2ca7cc37ac2cb3c96/skills/quest/SKILL.md) · 499★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: quest
description: >
  Background job scheduling with sails-hook-quest for Sails.js applications.
  Use this skill when creating, scheduling, or managing background jobs,
  cron tasks, recurring scripts, or any deferred/periodic work in a Sails.js application.
metadata:
  author: sailscastshq
  version: '1.0.0'
  tags: quest, jobs, scheduling, cron, background, scripts, sails
---

# Quest — Background Job Scheduling

Quest is a job scheduling hook for Sails.js that turns scripts in the `scripts/` directory into scheduled background jobs. Each job runs as an isolated child process via `sails run`, with full access to models, helpers, and configuration.

## When to Use

Use this skill when:

- Creating background jobs or scheduled tasks
- Setting up cron schedules, recurring intervals, or one-time delayed execution
- Defining job scripts with inputs and overlap prevention
- Using the `sails.quest` API to manage jobs at runtime
- Listening to job lifecycle events (start, complete, error)
- Configuring the console environment for lightweight job execution

## Rules

Read individual rule files for detailed explanations and code examples:

- [rules/getting-started.md](rules/get
```

</details>
