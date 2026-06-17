---
name: inseq-team__inseq
source: https://github.com/inseq-team/inseq/blob/a269ee8fbc65f9079109856e0f995e39a6333a8b/CLAUDE.md
repo: inseq-team/inseq
kind: claude-md
stars: 467
last_pushed: 2026-04-25T15:29:40Z
license: apache-2.0
score: 9
domains: [ml-research, python-package, cli-tools]
tags: [architecture-patterns, extension-guide]
curated: 2026-06-15
curated_by: config-scout
---

# inseq-team/inseq — claude-md

**Why it's worth keeping:** Includes high-value 'Adding New Components' templates and a task-to-file mapping table that guides the AI on where to implement new features.

**Summary:** Provides deep architectural context, extension patterns, and specific toolchain instructions for a complex ML library.

**Source credibility:** High; well-maintained repository with significant social proof (467 stars) and recent activity.

**Recency:** Current; utilizes modern Python tooling like uv, ruff, and strict mypy.

**Source:** [inseq-team/inseq/CLAUDE.md](https://github.com/inseq-team/inseq/blob/a269ee8fbc65f9079109856e0f995e39a6333a8b/CLAUDE.md) · 467★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Inseq Project Documentation

## Project Overview

**Inseq** is a PyTorch-based interpretability toolkit for analyzing and explaining sequence generation models. It democratizes access to common post-hoc interpretability analyses for generative language models.

- **Version:** 0.7.1
- **Python Support:** 3.10, 3.11, 3.12, 3.13
- **License:** Apache License 2.0
- **Documentation:** https://inseq.org
- **Repository:** https://github.com/inseq-team/inseq

## Quick Start Commands

```bash
# Download and install uv package manager
make uv-download

# Install package (uses uv sync)
make install

# Install with all development dependencies (uses uv sync --all-extras)
make install-dev

# Run all tests
make test

# Run tests without GPU
make test-cpu

# Run fast tests only (skip slow tests)
make fast-test

# Check code style
make check-style

# Auto-format code
make fix-style

# Build documentation
make build-docs

# Serve docs locally
make serve-docs
```

## Dependency Management

This project uses [uv](https://github.com/astral-sh/uv) for fast, reliable Python package management:

- **`uv sync`** - Install core dependencies from `pyproject.toml`
- **`uv sync --all-extras`** -
```

</details>
