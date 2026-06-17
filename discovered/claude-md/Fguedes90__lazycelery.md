---
name: Fguedes90__lazycelery
source: https://github.com/Fguedes90/lazycelery/blob/959810dc1c9f118321e2f0bb1dffba9b640e1e86/CLAUDE.md
repo: Fguedes90/lazycelery
kind: claude-md
stars: 55
last_pushed: 2026-06-03T01:26:17Z
license: mit
score: 9
domains: [cli-tools, rust, backend]
tags: [architecture-map, command-reference, status-tracking]
curated: 2026-06-15
curated_by: config-scout
---

# Fguedes90/lazycelery — claude-md

**Why it's worth keeping:** The data flow diagram and module responsibility sections provide high-level structural reasoning, while specific command groupings prevent tool hallucination.

**Summary:** Provides deep architectural context, comprehensive development commands via mise, and clear implementation/testing strategies.

**Source credibility:** High; well-documented project with significant GitHub social proof.

**Recency:** Current; uses modern development tools like mise and specialized Rust workflows.

**Source:** [Fguedes90/lazycelery/CLAUDE.md](https://github.com/Fguedes90/lazycelery/blob/959810dc1c9f118321e2f0bb1dffba9b640e1e86/CLAUDE.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LazyCelery is a terminal UI for monitoring and managing Celery workers and tasks, inspired by lazydocker/lazygit. This is a Rust project with a fully functional architecture and UI framework. Currently implementing real Celery protocol integration to replace mock data systems.

## Development Commands

```bash
# Core development commands using mise:
mise run dev                            # Run with auto-reload (auto-starts Redis)
mise run test                           # Run all tests
mise run test-watch                     # Run tests in watch mode
mise run fmt                            # Format code
mise run lint                           # Lint code (clippy)
mise run audit                          # Security audit
mise run pre-commit                     # Run all checks before committing

# Setup and environment:
mise run setup                          # Setup development environment
mise run redis-start                    # Start Redis server via Docker
mise run redis-stop                     # Stop Redis server

# Git hooks setup (run once
```

</details>
