---
name: sanskarbasnet__fstack__skill-tmpl
source: https://github.com/sanskarbasnet/fstack/blob/ef2b354205a8c146330d3e86259807b1aa0caaf9/retro/SKILL.md.tmpl
repo: sanskarbasnet/fstack
kind: skill
stars: 1
last_pushed: 2026-05-05T19:30:40Z
license: other
score: 9
domains: [cli-tools, devops, productivity]
tags: [retrospective, git-analysis, metrics]
curated: 2026-06-16
curated_by: config-scout
---

# sanskarbasnet/fstack — skill

**Why it's worth keeping:** It demonstrates advanced data-gathering techniques using specific `git log` formatting and implements robust time-window math for precise reporting.

**Summary:** A sophisticated engineering retrospective tool that automates the aggregation of git history, code metrics, and team contributions.

**Source credibility:** High technical depth; while stars are low, the sophistication of the shell commands suggests a professional engineering tool.

**Recency:** Very current; integrates modern agentic patterns like gbrain context loading and advanced shell execution.

**Source:** [sanskarbasnet/fstack/retro/SKILL.md.tmpl](https://github.com/sanskarbasnet/fstack/blob/ef2b354205a8c146330d3e86259807b1aa0caaf9/retro/SKILL.md.tmpl) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: retro
preamble-tier: 2
version: 2.0.0
description: |
  Weekly engineering retrospective. Analyzes commit history, work patterns,
  and code quality metrics with persistent history and trend tracking.
  Team-aware: breaks down per-person contributions with praise and growth areas.
  Use when asked to "weekly retro", "what did we ship", or "engineering retrospective".
  Proactively suggest at the end of a work week or sprint. (fstack)
allowed-tools:
  - Bash
  - Read
  - Write
  - Glob
  - AskUserQuestion
triggers:
  - weekly retro
  - what did we ship
  - engineering retrospective
gbrain:
  schema: 1
  context_queries:
    - id: prior-retros
      kind: filesystem
      glob: "~/.fstack/projects/{repo_slug}/retros/*.md"
      sort: mtime_desc
      limit: 5
      render_as: "## Prior retros for this project"
    - id: recent-timeline
      kind: filesystem
      glob: "~/.fstack/projects/{repo_slug}/timeline.jsonl"
      tail: 30
      render_as: "## Recent timeline events"
    - id: recent-learnings
      kind: filesystem
      glob: "~/.fstack/projects/{repo_slug}/learnings.jsonl"
      tail: 10
      render_as: "## Recent learnings"
---

{{PREAMBLE}}

{{BASE_BRANCH_DETE
```

</details>
