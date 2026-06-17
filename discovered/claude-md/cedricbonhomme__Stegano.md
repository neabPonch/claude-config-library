---
name: cedricbonhomme__Stegano
source: https://github.com/cedricbonhomme/Stegano/blob/f7745e85265f9e13c2df12446f91f62554203ba4/CLAUDE.md
repo: cedricbonhomme/Stegano
kind: claude-md
stars: 591
last_pushed: 2026-06-05T05:29:17Z
license: gpl-3.0
score: 8
domains: [python, security, image-processing]
tags: [architecture-mapping, workflow-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# cedricbonhomme/Stegano — claude-md

**Why it's worth keeping:** The 'Architecture' and 'Key Patterns' sections are excellent templates for showing an LLM how different submodules interact and the expected API shape.

**Summary:** Provides highly detailed architectural mapping and explicit development workflows for testing, type checking, and documentation.

**Source credibility:** Strong; a popular Python project with nearly 600 stars.

**Recency:** Modern; uses contemporary tooling like mypy, pre-commit, and pyproject.toml.

**Source:** [cedricbonhomme/Stegano/CLAUDE.md](https://github.com/cedricbonhomme/Stegano/blob/f7745e85265f9e13c2df12446f91f62554203ba4/CLAUDE.md) · 591★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Stegano is a pure Python steganography module that provides multiple techniques for hiding messages in images and audio files. The codebase is structured around independent steganography techniques, each with a `hide()` and `reveal()` interface.

## Development Commands

### Testing
```bash
# Run all tests
python -m unittest discover -v

# Run a single test file
python -m unittest tests.test_lsb -v

# Run a specific test case
python -m unittest tests.test_lsb.TestLSB.test_hide_and_reveal -v
```

### Type Checking
```bash
# Run mypy static type checker
mypy stegano
```

### Code Quality
```bash
# Run pre-commit hooks manually
pre-commit run --all-files

# Install pre-commit hooks
pre-commit install
```

### Building Documentation
```bash
cd docs
pip install -r requirements.txt
make html
```

## Architecture

### Core Steganography Techniques

The module provides four main steganography techniques, each in its own submodule:

1. **LSB (Least Significant Bit)** - `stegano/lsb/`
   - Primary technique using pixel LSB manipulation
   - Supports custom generat
```

</details>
