---
name: Natfii__UnrealClaude__claude-default
source: https://github.com/Natfii/UnrealClaude/blob/9f12f2edf5484a2da48c675c12a73e4ebe0ae4da/UnrealClaude/CLAUDE.md.default
repo: Natfii/UnrealClaude
kind: claude-md
stars: 756
last_pushed: 2026-05-16T13:38:30Z
license: unknown
score: 9
domains: [game-dev, agents-ai, cli-tools, mcp-integration]
tags: [unreal-engine, concurrency-management, tool-routing, mcp]
curated: 2026-06-15
curated_by: config-scout
---

# Natfii/UnrealClaude — claude-md

**Why it's worth keeping:** The 'Parallel Tool Execution' table and the mandatory 'Tool Router' pattern are elite techniques for preventing race conditions and managing concurrency limits in complex environments.

**Summary:** Provides deep integration instructions for an Unreal Engine 5.7 MCP-based toolset, emphasizing agentic control over the editor state.

**Source credibility:** High; demonstrated by high star count (756) and recent maintenance history.

**Recency:** Very current, referencing specific tool versions (v1.4.4) and targeting modern engine versions.

**Source:** [Natfii/UnrealClaude/UnrealClaude/CLAUDE.md.default](https://github.com/Natfii/UnrealClaude/blob/9f12f2edf5484a2da48c675c12a73e4ebe0ae4da/UnrealClaude/CLAUDE.md.default) · 756★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# UnrealClaude - Claude Code Instructions for Unreal Engine 5.7

This file provides guidance to Claude Code when working with the UnrealClaude plugin and Unreal Engine 5.7 projects.

## Setup

Copy this file to `CLAUDE.md` in the same directory and customize the build paths for your system.

## Project Overview

**UnrealClaude** is an Unreal Engine 5.7 plugin that provides MCP (Model Context Protocol) integration, enabling Claude AI to interact directly with the Unreal Editor via REST API tools.

### MCP Tool Priority

When working with Unreal Editor content, ALWAYS prefer MCP tools over filesystem tools:
- Use `asset_search` instead of Glob/Grep to find assets
- Use `spawn_actor` instead of writing Python scripts to create actors
- Use `get_level_actors` instead of reading level files to see what's in a scene
- Use `blueprint_query` instead of reading .uasset files to inspect blueprints
- MCP tools operate on the live editor state — filesystem tools see serialized data

**Note on parameter names:** as of v1.4.4, `asset_search` uses `class_filter` (formerly `asset_type`) and `name_pattern` (formerly `search_term`). The old names still work via aliases but emit deprecation warnings
```

</details>
