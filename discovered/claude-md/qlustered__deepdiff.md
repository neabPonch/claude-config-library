---
name: qlustered__deepdiff
source: https://github.com/qlustered/deepdiff/blob/c59636cda63cd3951777208c783285e6bf634159/CLAUDE.md
repo: qlustered/deepdiff
kind: claude-md
stars: 2512
last_pushed: 2026-05-15T20:15:51Z
license: other
score: 9
domains: [python, cli-tools]
tags: [uv, testing-patterns, environment-management]
curated: 2026-06-14
curated_by: config-scout
---

# qlustered/deepdiff — claude-md

**Why it's worth keeping:** The 'Common Pitfalls' section is excellent at preventing agent errors, and the explicit use of command chains (source venv && command) ensures correct execution context.

**Summary:** A highly practical guide for maintaining a Python development environment using modern tooling like uv and pyright.

**Source credibility:** High; the source project is a popular, well-maintained library with significant GitHub star count.

**Recency:** Current; it uses modern Python standards like uv and pyright which are highly relevant to today's development workflows.

**Source:** [qlustered/deepdiff/CLAUDE.md](https://github.com/qlustered/deepdiff/blob/c59636cda63cd3951777208c783285e6bf634159/CLAUDE.md) · 2512★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DeepDiff is a Python library for deep comparison, searching, and hashing of Python objects. It provides:
- **DeepDiff**: Deep difference detection between objects
- **DeepSearch**: Search for objects within other objects  
- **DeepHash**: Content-based hashing for any object
- **Delta**: Git-like diff objects that can be applied to other objects
- **CLI**: Command-line interface via `deep` command

## Development Commands

### Setup
```bash
# Install with all development dependencies
uv pip install -e ".[cli,coverage,dev,docs,static,test]"
# OR using uv (recommended)
uv sync --all-extras
```

**Virtual Environment**: Activate with `source ~/.venvs/deep/bin/activate` before running tests or Python commands


### Testing
```bash
# Run tests with coverage
source ~/.venvs/deep/bin/activate && pytest --cov=deepdiff --cov-report term-missing

# Run tests including slow ones
source ~/.venvs/deep/bin/activate && pytest --cov=deepdiff --runslow

# Run single test file
source ~/.venvs/deep/bin/activate && pytest tests/test_diff_text.py

# Run tests across
```

</details>
