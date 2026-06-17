---
name: andyjmorgan__DonkeyWork-Agents
source: https://github.com/andyjmorgan/DonkeyWork-Agents/blob/4f2d5b93e1ea750de9d594ed30f1d6efeb7f0457/claude.md
repo: andyjmorgan/DonkeyWork-Agents
kind: claude-md
stars: 0
last_pushed: 2026-06-03T15:47:52Z
license: unknown
score: 9
domains: [backend-api, agents-ai, workflow-automation]
tags: [agentic-workflow, .net, mcp, parallelization, task-management]
curated: 2026-06-14
curated_by: config-scout
---

# andyjmorgan/DonkeyWork-Agents — claude-md

**Why it's worth keeping:** The explicit 'Assess -> Plan (as Note) -> Execute -> Verify' workflow and the sophisticated guidelines for safe parallelization are world-class templates for agent orchestration.

**Summary:** This file defines a rigorous autonomous agent lifecycle that uses MCP tools to manage project state, task prioritization, and progress tracking.

**Source credibility:** Low social proof/stars, but the content demonstrates a high level of technical sophistication in agentic workflows.

**Recency:** Extremely current; utilizes modern .NET 10 and advanced MCP tool patterns common in today's Claude Code ecosystem.

**Source:** [andyjmorgan/DonkeyWork-Agents/claude.md](https://github.com/andyjmorgan/DonkeyWork-Agents/blob/4f2d5b93e1ea750de9d594ed30f1d6efeb7f0457/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Project is a Modular monolith.

## Prerequisites

- **.NET 10 SDK** is required to build and test this project
- Install via script: `curl -sSL https://dot.net/v1/dotnet-install.sh | bash /dev/stdin --channel 10.0`
- After installation, add to PATH: `export PATH="$HOME/.dotnet:$PATH"`

## DonkeyWork Project Management Workflow

When assigned a project or milestone via the DonkeyWork MCP tools, follow this workflow:

### Determining What to Work On

Before starting work, assess the full backlog:

1. **List all projects** - Use `mcp__donkeywork__projects_list` to see all projects
2. **List milestones and tasks** - For each active project, use `mcp__donkeywork__milestones_list` and `mcp__donkeywork__tasks_list_by_project` to see all work items
3. **Evaluate priorities** - Consider:
   - Status (items already `InProgress` take precedence)
   - Due dates
   - Dependencies (blocked items wait, blockers come first)
   - Priority field on tasks (`Critical` > `High` > `Medium` > `Low`)
   - Sort order
4. **Adjust priorities** - Use update tools to shift `sortOrder` or `priority` of items as appropriate based on the current state
5. **Select next item** - Pick the highest priority unblocked
```

</details>
