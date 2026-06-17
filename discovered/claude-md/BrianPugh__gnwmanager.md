---
name: BrianPugh__gnwmanager
source: https://github.com/BrianPugh/gnwmanager/blob/8830140832d51ad95c347ac386263abc20965e1f/CLAUDE.md
repo: BrianPugh/gnwmanager
kind: claude-md
stars: 91
last_pushed: 2026-06-08T16:42:41Z
license: apache-2.0
score: 9
domains: [cli-tools, embedded-systems, python]
tags: [python, stm32, firmware, uv]
curated: 2026-06-15
curated_by: config-scout
---

# BrianPugh/gnwmanager — claude-md

**Why it's worth keeping:** It includes specific 'Common Commands' that reduce AI trial-and-error during testing/linting and explains complex architectural details like the memory-mapped communication protocol.

**Summary:** Provides a comprehensive guide for a hybrid Python CLI and embedded STM32 firmware project. It covers environment setup, build commands, architectural patterns, and strict coding standards.

**Source credibility:** High; well-maintained repository with active development and clear technical depth.

**Recency:** Highly current, utilizing modern tooling like uv, ruff, and pyright.

**Source:** [BrianPugh/gnwmanager/CLAUDE.md](https://github.com/BrianPugh/gnwmanager/blob/8830140832d51ad95c347ac386263abc20965e1f/CLAUDE.md) · 91★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GnWManager is a Game & Watch device manager — a Python CLI tool + STM32 firmware that communicates with Game & Watch hardware via debug probes (STLink, JLink, PyOCD, DAPLink, Raspberry Pi). It handles firmware flashing, filesystem management (LittleFS on external flash), device unlocking/locking, screenshots, monitoring, and GDB debugging.

## Development Setup

```bash
uv sync                     # Create venv and install dependencies
uv run pre-commit install   # Install git hooks (ruff, black, codespell, pyright)
```

## Common Commands

```bash
# Python tests
uv run pytest                      # Run all tests
uv run pytest tests/test_foo.py    # Run a single test file
uv run pytest tests/test_foo.py::test_bar  # Run a single test
uv run pytest -x                   # Stop on first failure

# Linting & formatting
uv run ruff check gnwmanager/      # Lint
uv run ruff check --fix gnwmanager/  # Lint with auto-fix
uv run black gnwmanager/ tests/    # Format (line-length=120)

# Build STM32 firmware (requires arm-none-eabi-gcc)
make -j4
```

</details>
