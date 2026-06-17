---
name: RchGrav__claudebox
source: https://github.com/RchGrav/claudebox/blob/a7799bb5a7801f03f1343009b1cdfdaaa83c7fb6/CLAUDE.md
repo: RchGrav/claudebox
kind: claude-md
stars: 1098
last_pushed: 2025-08-31T01:14:07Z
license: mit
score: 9
domains: [cli-tools, devops, shell-scripting]
tags: [bash, docker, error-handling, constraints]
curated: 2026-06-15
curated_by: config-scout
---

# RchGrav/claudebox — claude-md

**Why it's worth keeping:** It uses highly effective 'Wrong vs. Correct' code examples to prevent subtle errors caused by `set -e` and defines exact technical constraints (like Bash 3.2 compatibility) to preempt LLM hallucinations.

**Summary:** This file establishes strict operational guardrails for maintaining a complex Bash/Docker environment, specifically preventing breaking changes in container management and shell execution logic.

**Source credibility:** High; part of a popular specialized developer tool with over 1,000 stars.

**Recency:** The content is highly relevant to current containerized CLI development workflows.

**Source:** [RchGrav/claudebox/CLAUDE.md](https://github.com/RchGrav/claudebox/blob/a7799bb5a7801f03f1343009b1cdfdaaa83c7fb6/CLAUDE.md) · 1098★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

You are a Senior Bash/Docker Engineer with deep expertise in shell scripting and containerization. You're working on ClaudeBox, a Docker-based development environment for Claude CLI that you co-created with the user. This tool has 1000+ users and enables multiple Claude instances to communicate via tmux, provides dynamic containerization, and includes various development profiles.

## Critical Requirements

- **Bash 3.2 compatibility ONLY** - this ensures it works on both macOS and Linux
- **Preserve ALL existing functionality** - breaking changes have caused days of lost work
- **Read and understand code thoroughly** before suggesting any modifications

## CRITICAL DESIGN DECISIONS - DO NOT CHANGE

### Container Management
- **Named containers WITH --rm flag** - This is intentional and works perfectly
- **Containers are ephemeral** - They are created, run, and auto-delete on exit
- **Slot system tracks availability** - Each slot gets a unique container name
- **DO NOT remove --rm flag** - Containers must clean themselves up
- **DO NOT try to delete containers on sta
```

</details>
