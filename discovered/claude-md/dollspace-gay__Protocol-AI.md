---
name: dollspace-gay__Protocol-AI
source: https://github.com/dollspace-gay/Protocol-AI/blob/7cdc36b4aa71df58d17a35ddf0d9d3e85390db75/Claude.md
repo: dollspace-gay/Protocol-AI
kind: claude-md
stars: 4
last_pushed: 2025-11-21T13:11:42Z
license: mit
score: 7
domains: [cli-tools, agents-ai, workflow-automation]
tags: [task-management, agentic-workflows, cli]
curated: 2026-06-14
curated_by: config-scout
---

# dollspace-gay/Protocol-AI — claude-md

**Why it's worth keeping:** It defines an 'agent-ready' protocol (via `bd ready`) that allows the AI to autonomously identify unblocked tasks within a structured hierarchy.

**Summary:** Mandates a dependency-aware CLI issue tracker (bd) instead of markdown files to manage task state and agent workflows.

**Source credibility:** 4 stars; appears to be an experimental or niche tool developed by a single contributor.

**Recency:** Current; its focus on agentic state management is highly relevant to Claude Code workflows.

**Source:** [dollspace-gay/Protocol-AI/Claude.md](https://github.com/dollspace-gay/Protocol-AI/blob/7cdc36b4aa71df58d17a35ddf0d9d3e85390db75/Claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Quick Start

Instructions for Claude
For all work in this repository, you must use the beads issue tracker.
Use the bd command-line tool to create, manage, and close issues.
Do not use markdown files for creating to-do lists or for tracking your work. All issues and bugs are to be tracked via bd.

bd - Dependency-Aware Issue Tracker

Issues chained together like beads.

GETTING STARTED
  bd init   Initialize bd in your project
            Creates .beads/ directory with project-specific database        
            Auto-detects prefix from directory name (e.g., myapp-1, myapp-2)

  bd init --prefix api   Initialize with custom prefix
            Issues will be named: api-1, api-2, ...

CREATING ISSUES
  bd create "Fix login bug"
  bd create "Add auth" -p 0 -t feature
  bd create "Write tests" -d "Unit tests for auth" --assignee alice

VIEWING ISSUES
  bd list       List all issues
  bd list --status open  List by status
  bd list --priority 0  List by priority (0-4, 0=highest)
  bd show bd-1       Show issue details

MANAGING DEPENDENCIES
  bd dep add bd-1 bd-2     Add dependency (bd-2 blocks bd-1)
  bd dep tree bd-1  Visualize dependency tree
  bd dep cycles      Detect circular
```

</details>
