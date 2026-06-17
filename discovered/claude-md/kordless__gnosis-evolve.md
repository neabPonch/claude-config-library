---
name: kordless__gnosis-evolve
source: https://github.com/kordless/gnosis-evolve/blob/5532b82b5a64a31b80b259b2c65f48a02c8873bb/claude.md
repo: kordless/gnosis-evolve
kind: claude-md
stars: 57
last_pushed: 2025-06-20T18:46:14Z
license: other
score: 8
domains: [agents-ai, cli-tools, automation]
tags: [self-modifying, mcp, attention-management]
curated: 2026-06-16
curated_by: config-scout
---

# kordless/gnosis-evolve — claude-md

**Why it's worth keeping:** Uses 'Meta-Context' to manage attention/circularity issues and enforces strict procedural distinction between tool registration and file writing.

**Summary:** Instructions for a self-modifying agentic system where Claude creates and installs its own Python-based MCP tools.

**Source credibility:** Niche project with moderate star count (57) for a specialized toolset.

**Recency:** 12 months old; principles are evergreen, but specific MCP implementations may have evolved.

**Source:** [kordless/gnosis-evolve/claude.md](https://github.com/kordless/gnosis-evolve/blob/5532b82b5a64a31b80b259b2c65f48a02c8873bb/claude.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# EvolveMCP Project Guide for Claude

## Purpose of This Document

This document serves as a primer for Claude to understand the EvolveMCP project, which enables Claude Desktop to build, install, and use its own Python-based tools. When starting a new session with this project, Claude should:

1. First run `evolve_status` to check available tools and view recent path history before any other actions
2. Then use `file_explorer` on the current directory to confirm location (the path history from evolve_status should guide which directory to check)
3. Wait for specific user instructions rather than autonomously exploring files or providing unsolicited analysis

## Important Meta-Context: Claude as Both User and Developer

**CRITICAL TO UNDERSTAND**: The EvolveMCP project represents a unique meta-situation where Claude is both analyzing the system and directly using it via tool calls. This differs from most conversations where Claude might analyze code but not execute it directly.

- Claude is actively using the EvolveMCP tools through function calls in this conversation
- The tools being discussed are the same tools Claude is calling
- When Claude calls `evolve_status` or `file_explor
```

</details>
