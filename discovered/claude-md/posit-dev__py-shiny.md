---
name: posit-dev__py-shiny
source: https://github.com/posit-dev/py-shiny/blob/3a09844f26f5f084ff1159aa544594dde62b0460/CLAUDE.md
repo: posit-dev/py-shiny
kind: claude-md
stars: 1724
last_pushed: 2026-06-11T20:00:23Z
license: mit
score: 9
domains: [web-framework, python, frontend-interop]
tags: [architecture-heavy, command-rich, reactive-programming]
curated: 2026-06-15
curated_by: config-scout
---

# posit-dev/py-shiny — claude-md

**Why it's worth keeping:** It explains 'how to think' about the framework (e.g., push-pull reactivity and Express vs Core mode), which prevents AI from introducing logic errors, rather than just listing commands.

**Summary:** Provides comprehensive development commands alongside deep architectural mental models crucial for understanding the reactive system and execution modes.

**Source credibility:** High; comes from a major, highly-starred library (py-shiny) maintained by Posit.

**Recency:** Very current; includes specific workflows for modern testing frameworks like Playwright and esbuild.

**Source:** [posit-dev/py-shiny/CLAUDE.md](https://github.com/posit-dev/py-shiny/blob/3a09844f26f5f084ff1159aa544594dde62b0460/CLAUDE.md) · 1724★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

py-shiny is a Python web framework for building reactive web applications. It maintains feature parity with Shiny for R, often porting UI components from the R bslib package. The codebase consists of Python server-side code, TypeScript/JavaScript client-side code, and vendored assets from upstream packages.

## Development Commands

### Essential Commands
```bash
# Install dev dependencies
pip install -e ".[dev,test,doc]"

# Format code (always run before committing)
make format              # Auto-fix with black and isort
make check-format        # Check only

# Type checking
make check-types         # Run pyright (requires typings)

# Run tests
make test                # Unit tests only (pytest)
make playwright          # All end-to-end tests (slow)
make playwright-shiny SUB_FILE="inputs/test_foo.py"  # Single test

# Comprehensive checks
make check               # Format, lint, types, unit tests
make check-fix           # Same but auto-fixes formatting
```

### Asset Management
```bash
# Vendor assets from upstream (bslib, shiny, sass, htmltools)
make
```

</details>
