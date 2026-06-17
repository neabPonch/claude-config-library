---
name: vstorm-co__full-stack-ai-agent-template
source: https://github.com/vstorm-co/full-stack-ai-agent-template/blob/7ec4906c916e82d37023291be84af9bd110f34d9/CLAUDE.md
repo: vstorm-co/full-stack-ai-agent-template
kind: claude-md
stars: 1408
last_pushed: 2026-06-13T23:32:31Z
license: mit
score: 9
domains: [cli-tools, backend-api, ai-agents, full-stack]
tags: [template-generator, architecture-map, fastapi]
curated: 2026-06-15
curated_by: config-scout
---

# vstorm-co/full-stack-ai-agent-template — claude-md

**Why it's worth keeping:** The tree-based folder visualization provides immediate spatial awareness, while 'Key Design Decisions' proactively prevents pattern violations by defining the 'source of truth' for architecture.

**Summary:** A comprehensive architectural blueprint mapping the CLI generator logic alongside its generated project structure. It provides essential command context and high-level design constraints.

**Source credibility:** High-quality open source with 1.4k stars and active maintenance.

**Recency:** Up-to-date with modern tooling like uv and Next.js 15.

**Source:** [vstorm-co/full-stack-ai-agent-template/CLAUDE.md](https://github.com/vstorm-co/full-stack-ai-agent-template/blob/7ec4906c916e82d37023291be84af9bd110f34d9/CLAUDE.md) · 1408★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Full-Stack AI Agent Template** is an interactive CLI tool that generates production-ready FastAPI + Next.js projects with AI agents, RAG, and 20+ enterprise integrations. Uses Cookiecutter templates with Jinja2 conditionals.

## Commands

```bash
# Install dependencies
uv sync

# Run tests
uv run pytest

# Run single test
uv run pytest tests/test_file.py::test_name -v

# Linting and formatting
uv run ruff check . --fix
uv run ruff format .

# Type checking
uv run ty check
```

## CLI Usage

```bash
# Interactive wizard (default)
fastapi-fullstack

# Quick project creation
fastapi-fullstack create my_project --database postgresql

# With RAG
fastapi-fullstack create my_project --ai-framework pydantic_ai --rag --database postgresql --task-queue celery

# List available options
fastapi-fullstack templates
```

## Architecture

### Core Modules (`fastapi_gen/`)

- **cli.py** - Click-based CLI: `new` (interactive, default), `create` (direct), `templates` (list options)
- **config.py** - Pydantic models: `ProjectConfig`, enums (`AIFrameworkType`, `LL
```

</details>
