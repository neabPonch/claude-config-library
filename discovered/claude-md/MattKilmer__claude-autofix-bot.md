---
name: MattKilmer__claude-autofix-bot
source: https://github.com/MattKilmer/claude-autofix-bot/blob/957ba70c3a58d43dbdf022b869a3eedaf94401da/claude.md
repo: MattKilmer/claude-autofix-bot
kind: claude-md
stars: 5
last_pushed: 2025-12-12T23:12:20Z
license: unknown
score: 9
domains: [agents-ai, automation, cli-tools, backend]
tags: [orchestration, agentic-pipeline, slack-integration]
curated: 2026-06-14
curated_by: config-scout
---

# MattKilmer/claude-autofix-bot — claude-md

**Why it's worth keeping:** It features a highly effective 'Critical Files' table explaining the *role* of each file rather than just its name, and uses a flow diagram to establish system mental models.

**Summary:** This document provides high-level architectural context for an automated agentic pipeline that bridges Slack to Git via Claude Code CLI.

**Source credibility:** High-quality specialized tool with 5 stars and specific technical depth.

**Recency:** Current; specifically tailored for recent Claude Code CLI agentic capabilities.

**Source:** [MattKilmer/claude-autofix-bot/claude.md](https://github.com/MattKilmer/claude-autofix-bot/blob/957ba70c3a58d43dbdf022b869a3eedaf94401da/claude.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Context Document - Claude AutoFix Bot

> **Purpose:** This file provides comprehensive context for LLM agents (Claude, GPT, etc.) working on this codebase. Read this FIRST before making any changes.

---

## Project Overview

**Name:** Claude AutoFix Bot
**Type:** Production-ready AI-powered development automation system
**Status:** MVP complete with Claude Code CLI, deployable on Railway
**Repository:** https://github.com/MattKilmer/claude-autofix-bot
**Deployment Platform:** Railway (requires persistent server for Claude CLI)

### What This System Does

This is an **automated code fixing pipeline** that:

1. **Monitors** a Slack channel for bug reports/feature requests (natural language)
2. **Processes Images** - Analyzes attached screenshots for visual context (requires `files:read` scope)
3. **Analyzes** your codebase using Claude Code CLI (full agentic capabilities)
4. **Generates** code fixes using agentic tools (Read, Edit, Bash, Glob, Grep)
5. **Creates** a new Git branch with semantic naming (`fix/`, `feat/`, etc.)
6. **Commits** changes with descriptive messages
7. **Pushes** to GitHub and creates a Pull Request
8. **Reports** back to Slack with PR link + cost st
```

</details>
