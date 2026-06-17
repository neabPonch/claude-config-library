---
name: agude__wayback-machine-archiver
source: https://github.com/agude/wayback-machine-archiver/blob/a1c49b767a7eb60c36c57b36ec6d9732d3e985bc/CLAUDE.md
repo: agude/wayback-machine-archiver
kind: claude-md
stars: 86
last_pushed: 2026-06-09T16:25:32Z
license: mit
score: 8
domains: [cli-tools, python]
tags: [python, automation, api]
curated: 2026-06-15
curated_by: config-scout
---

# agude/wayback-machine-archiver — claude-md

**Why it's worth keeping:** The 'Workflow Pattern' section is highly transferable; it explains state transitions and error handling strategies which are difficult for AI to infer from code alone. It also includes granular test execution patterns.

**Summary:** Combines essential development commands with a high-level architectural breakdown that explains how logic flows through the system.

**Source credibility:** A niche but active utility repository with clear, purposeful documentation.

**Recency:** Current; follows modern Python development practices.

**Source:** [agude/wayback-machine-archiver/CLAUDE.md](https://github.com/agude/wayback-machine-archiver/blob/a1c49b767a7eb60c36c57b36ec6d9732d3e985bc/CLAUDE.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Wayback Machine Archiver is a CLI tool to submit web pages to the Internet Archive's Wayback Machine using the authenticated SPN2 API. It requires Internet Archive S3-style API keys (via `.env` file or environment variables).

## Development Commands

```bash
# Install for development
pip install -e ".[dev]"

# Run tests
pytest

# Run a single test file
pytest tests/test_cli.py

# Run a specific test
pytest tests/test_cli.py::test_version_action_exits

# Run the CLI
archiver --help
```

## Architecture

The codebase follows a layered architecture in `src/wayback_machine_archiver/`:

- **archiver.py** - Entry point (`main()`). Loads credentials from environment, gathers URLs from CLI args/sitemaps/files, and orchestrates the workflow.
- **cli.py** - Argument parser definition. All CLI flags including SPN2 API options are defined here.
- **clients.py** - `SPN2Client` class handles HTTP communication with the Internet Archive's SPN2 API (submit captures, check status, batch status checks).
- **workflow.py** - `run_archive_workflow()` manages the mai
```

</details>
