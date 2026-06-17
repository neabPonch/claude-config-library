---
name: beaufour__flickr-download
source: https://github.com/beaufour/flickr-download/blob/e5516da3feb31c03024571ad8ea674804f121922/CLAUDE.md
repo: beaufour/flickr-download
kind: claude-md
stars: 257
last_pushed: 2026-05-19T22:19:11Z
license: apache-2.0
score: 9
domains: [cli-tools, python]
tags: [command-driven, architecture-focus]
curated: 2026-06-15
curated_by: config-scout
---

# beaufour/flickr-download — claude-md

**Why it's worth keeping:** It provides explicit command sequences for testing and linting via 'uv', and uses an architecture section to explain design patterns like the Strategy pattern to prevent logic errors.

**Summary:** A high-quality guide that bridges operational commands with architectural mental models for a Python CLI tool.

**Source credibility:** High; the repository is well-maintained and shows active development with modern tooling.

**Recency:** Very current; utilizes modern Python standards like 'uv' and recent Python versions.

**Source:** [beaufour/flickr-download/CLAUDE.md](https://github.com/beaufour/flickr-download/blob/e5516da3feb31c03024571ad8ea674804f121922/CLAUDE.md) · 257★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Flickr Download is a command-line utility for downloading photos from Flickr. It supports downloading individual photos, photosets, or all photos from a user, with OAuth authentication for private/restricted content.

## Development Commands

```bash
# Install dependencies
uv sync --all-extras

# Run tests
uv run pytest -v

# Run tests with coverage
uv run coverage run -m pytest
uv run coverage html -d coverage

# Code quality checks (also run via pre-commit)
uv run ruff check flickr_download tests
uv run ruff format --check flickr_download tests
uv run mypy flickr_download

# Run all pre-commit hooks
uv run pre-commit run --all-files

# Run the CLI
uv run flickr_download [args]
```

## Architecture

### Main Package (`flickr_download/`)

- **flick_download.py** - Main entry point with CLI argument parsing, core download functions (`download_set`, `download_list`, `download_photo`, `download_user`, `download_user_photos`), and OAuth handling
- **filename_handlers.py** - Strategy pattern implementation for file naming (title, id, title_and_id, id_
```

</details>
