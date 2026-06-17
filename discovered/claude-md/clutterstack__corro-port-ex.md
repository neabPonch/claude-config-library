---
name: clutterstack__corro-port-ex
source: https://github.com/clutterstack/corro-port-ex/blob/06475b55ce688b2a152b1b58d3662e92c2c91211/CLAUDE.md
repo: clutterstack/corro-port-ex
kind: claude-md
stars: 0
last_pushed: 2025-10-16T00:16:17Z
license: unknown
score: 9
domains: [backend, distributed-systems, elixir-phoenix, cli-tools]
tags: [task-management, cluster-orchestration, agent-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# clutterstack/corro-port-ex — claude-md

**Why it's worth keeping:** The `bd` tool documentation teaches the AI how to manage its own state and dependencies; the command sections provide high-fidelity execution paths for complex system setups.

**Summary:** Provides a workflow for an agent-specific task tracker (`bd`) and detailed orchestration instructions for running a complex multi-node Elixir cluster.

**Source credibility:** High technical depth despite low repository visibility, suggesting a sophisticated local development environment.

**Recency:** Current; integrates seamlessly with modern agentic workflows and CLI tools.

**Source:** [clutterstack/corro-port-ex/CLAUDE.md](https://github.com/clutterstack/corro-port-ex/blob/06475b55ce688b2a152b1b58d3662e92c2c91211/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.


## Keeping track of work
Use the `bd` tool instead of markdown for all new work

### Using the bd tool

The `bd` tool is a dependency-aware issue tracker where issues are chained together like beads. It uses a local SQLite database that auto-syncs with git via JSONL exports.

**Getting started:**
```bash
# Initialize bd in your project (already done for this repo)
bd init                    # Auto-detects prefix from directory name
bd init --prefix api       # Custom prefix (issues named: api-1, api-2, ...)
```

**Creating issues:**
```bash
# Basic issue creation
bd create "Issue title" -d "Detailed description"

# With type, priority, and assignee
bd create "Add auth" -t feature -p 0 -d "Description" --assignee alice

# Issue types: bug, feature, task, epic, chore
bd create "Fix login bug" -t bug -d "Bug description"
```

**Managing dependencies:**
```bash
# Add dependency (bd-2 blocks bd-1, so bd-2 must complete first)
bd dep add bd-1 bd-2

# Visualize dependency tree
bd dep tree bd-1

# Detect circular dependencies
bd dep cycles
```

**Dependency types:**
- `bloc
```

</details>
