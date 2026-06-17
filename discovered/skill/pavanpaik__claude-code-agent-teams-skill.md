---
name: pavanpaik__claude-code-agent-teams-skill
source: https://github.com/pavanpaik/claude-code-agent-teams-skill/blob/d1d1adcbcd0156a263c8380653224adae1b06fc7/skill.md
repo: pavanpaik/claude-code-agent-teams-skill
kind: skill
stars: 2
last_pushed: 2026-02-08T12:22:32Z
license: mit
score: 8
domains: [agents-ai, cli-tools, orchestration]
tags: [multi-agent, task-coordination, tmux]
curated: 2026-06-16
curated_by: config-scout
---

# pavanpaik/claude-code-agent-teams-skill — skill

**Why it's worth keeping:** Implements a robust decentralized protocol for agent coordination via local file-system messages. The use of tmux panes for spawning subprocesses provides an excellent pattern for managing independent, visible sub-agents.

**Summary:** Orchestrates multiple Claude Code instances using shared task lists and JSON-based message inboxes for inter-agent communication.

**Source credibility:** Low star count (2), but the technical complexity indicates a highly sophisticated orchestration tool rather than a generic prompt.

**Recency:** Very recent (4 months ago) and aligns with current Claude Code capabilities.

**Source:** [pavanpaik/claude-code-agent-teams-skill/skill.md](https://github.com/pavanpaik/claude-code-agent-teams-skill/blob/d1d1adcbcd0156a263c8380653224adae1b06fc7/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Teams Skill

This skill enables Claude Code to orchestrate multiple AI agents working together as a team, with shared task lists, inter-agent messaging, and coordinated workflows.

## Description

The Agent Teams skill implements a native protocol for coordinating multiple Claude Code instances as a collaborative team. It provides:

- **Team Management**: Create and manage agent teams with shared configuration
- **Task Coordination**: Shared task lists with dependencies, ownership, and status tracking
- **Inter-Agent Messaging**: Direct messages, broadcasts, and protocol requests between teammates
- **Agent Spawning**: Launch new Claude Code teammates in tmux panes
- **Lifecycle Management**: Graceful shutdown, force termination, and cleanup

## When to Use

Use this skill when you need:

- Multiple AI agents working on different parts of a complex project simultaneously
- Coordinated workflows where agents need to communicate and share progress
- Parallel execution of independent tasks with dependency management
- A lead agent orchestrating and delegating work to specialized teammates

## Core Concepts

### Teams
- One team per session, stored in `~/.claude/teams/<team-nam
```

</details>
