---
name: stravalib__stravalib
source: https://github.com/stravalib/stravalib/blob/96d8ef63c7c80d2ebcb241ed6c20b814eaaad82d/CLAUDE.md
repo: stravalib/stravalib
kind: claude-md
stars: 987
last_pushed: 2026-06-01T12:35:42Z
license: apache-2.0
score: 9
domains: [python, api-client, library]
tags: [rest-api, nox, pydantic, testing-guide]
curated: 2026-06-15
curated_by: config-scout
---

# stravalib/stravalib — claude-md

**Why it's worth keeping:** Crucially warns against editing auto-generated files and explains the complex interaction between Client, Protocol, and Model layers to prevent structural errors.

**Summary:** A comprehensive technical guide for a Python API library that outlines architectural patterns, authentication logic, and specific development workflows.

**Source credibility:** High; a well-starred, actively maintained open-source library.

**Recency:** Very current; includes support for modern Python versions up to 3.14 and Pydantic v2.

**Source:** [stravalib/stravalib/CLAUDE.md](https://github.com/stravalib/stravalib/blob/96d8ef63c7c80d2ebcb241ed6c20b814eaaad82d/CLAUDE.md) · 987★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Stravalib is a Python library providing easy-to-use tools for accessing and downloading Strava data from the Strava V3 REST API. The library supports authentication, rate limiting, data access/download, and unit conversion through the Pint library.

## Development Commands

### Testing

Run all tests across all supported Python versions (3.10-3.14):
```bash
nox -s tests
```

Run tests for a specific Python version:
```bash
nox -s tests-3.11
```

Run a single test file:
```bash
pytest src/stravalib/tests/unit/test_client.py
```

Run a specific test:
```bash
pytest src/stravalib/tests/unit/test_client.py::test_name
```

### Type Checking

Run mypy type checking:
```bash
nox -s mypy
```

### Linting and Formatting

The project uses pre-commit hooks with ruff (linting), black (formatting), and codespell (spell checking).

Install pre-commit hooks:
```bash
pre-commit install --install-hooks
```

Run pre-commit on all files:
```bash
pre-commit run --all-files
```

Run a specific hook:
```bash
pre-commit run ruff --all-files
```

### Documentation

Build docs:
```

</details>
