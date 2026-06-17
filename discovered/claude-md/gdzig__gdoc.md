---
name: gdzig__gdoc
source: https://github.com/gdzig/gdoc/blob/62b467aab40bad9686d827f09cf429ca4600630e/CLAUDE.md
repo: gdzig/gdoc
kind: claude-md
stars: 8
last_pushed: 2026-05-17T08:38:01Z
license: mit
score: 9
domains: [cli-tools, systems-programming]
tags: [zig, build-system, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# gdzig/gdoc — claude-md

**Why it's worth keeping:** Includes an 'Expected Data Flow' section to aid agentic reasoning and prescribes specific commands for a non-standard task management tool (beads) instead of generic TODOs.

**Summary:** A high-density technical guide for a Zig CLI project that integrates build instructions, architectural data flow, and custom issue-tracking workflows.

**Source credibility:** Small but active niche project with recent maintenance.

**Recency:** Very current; reflects modern developer workflows using mise and Zig.

**Source:** [gdzig/gdoc/CLAUDE.md](https://github.com/gdzig/gdoc/blob/62b467aab40bad9686d827f09cf429ca4600630e/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

**Note**: This project uses [bd (beads)](https://github.com/steveyegge/beads) for issue tracking. Use `bd` commands instead of markdown TODOs. See AGENTS.md for workflow details.

## Project Overview

**gdoc** is a CLI documentation viewer for Godot API documentation, similar to `zigdoc`. It parses Godot's API documentation and displays it in the terminal with BBCode-to-Markdown conversion.

Key behavior:
- Requires `godot` executable to determine version and fetch XML class documentation
- Downloads XML docs from GitHub, parses them, and builds a markdown cache
- Converts BBCode documentation to Markdown using the `bbcodez` library for terminal display

## Build System

### Dependencies
- **Zig**: 0.15.1 (managed via mise)
- **ZLS**: 0.15.0 (Zig Language Server, managed via mise)
- **bbcodez**: BBCode parser/formatter library (fetched from git)

### Common Build Commands

```bash
# Build the executable
zig build

# Run the application
zig build run

# Run with arguments
zig build run -- <symbol>

# Run tests (both module and executable tests)
zig build test

# Insta
```

</details>
