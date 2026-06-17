---
name: ziwon__drizzler
source: https://github.com/ziwon/drizzler/blob/678966d6eda890195d04399b9e68df73d837808f/CLAUDE.md
repo: ziwon/drizzler
kind: claude-md
stars: 4
last_pushed: 2026-01-29T07:34:55Z
license: unknown
score: 9
domains: [cli-tools, backend-api, automation]
tags: [python, asyncio, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# ziwon/drizzler — claude-md

**Why it's worth keeping:** The explicit breakdown of complex logic (throttling/circuit breaking) and the use of a task runner provides elite context for AI reasoning.

**Summary:** Provides a deep architectural map and clear command workflows for both CLI and Web modes.

**Source credibility:** A specialized tool with high-quality, high-density documentation.

**Recency:** Current; references modern LLM providers and contemporary development patterns.

**Source:** [ziwon/drizzler/CLAUDE.md](https://github.com/ziwon/drizzler/blob/678966d6eda890195d04399b9e68df73d837808f/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Drizzler is an adaptive, host-aware HTTP fetcher and YouTube downloader with intelligent throttling, state persistence, and AI summarization. It operates in two modes: CLI for single-shot execution and Web SaaS (FastAPI + React) for job-based processing.

## Development Commands

```bash
# Setup
just install              # Install Python + Node dependencies
just install-hooks        # Install pre-commit hooks

# Code Quality
just lint                 # Ruff check + format check
just fix                  # Auto-fix linting issues
just type                 # MyPy type checking
just check                # Run lint + type together
just pre-commit           # Run all pre-commit hooks

# Running the Application
just run <URL> [options]  # CLI mode
just api                  # FastAPI backend (port 8000)
just ui                   # React dev server (Vite)
just web                  # Run both API and UI in parallel
just deploy-local         # Build UI + run unified server

# Docker
just docker-build         # Build image
just docker-run <URL>     # Run co
```

</details>
