---
name: fighthealthinsurance__fighthealthinsurance
source: https://github.com/fighthealthinsurance/fighthealthinsurance/blob/df0b882fb63cbe8e89e90613427d3085c9c6c139/CLAUDE.md
repo: fighthealthinsurance/fighthealthinsurance
kind: claude-md
stars: 147
last_pushed: 2026-06-15T05:27:18Z
license: other
score: 9
domains: [backend-api, machine-learning]
tags: [django, tox, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# fighthealthinsurance/fighthealthinsurance — claude-md

**Why it's worth keeping:** It provides explicit 'rules of engagement'—such as mandating the use of tox over direct pytest calls—and highlights critical patterns like encrypted field usage to prevent security errors.

**Summary:** A highly detailed guide for a Django/ML application that bridges high-level architecture with specific development guardrails.

**Source credibility:** High; the repository shows active maintenance and a sophisticated, production-ready technical stack.

**Recency:** Very current, featuring modern dependencies like Python 3.13 and React 19.

**Source:** [fighthealthinsurance/fighthealthinsurance/CLAUDE.md](https://github.com/fighthealthinsurance/fighthealthinsurance/blob/df0b882fb63cbe8e89e90613427d3085c9c6c139/CLAUDE.md) · 147★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Fight Health Insurance is a Django application that helps patients appeal health insurance denials. It combines a web interface with ML model integration to generate persuasive appeal letters. The system supports both synchronous and asynchronous workflows, with WebSocket streaming for real-time appeal generation.

## Build & Development Commands

```bash
# Install dependencies (Option A: Conda - recommended)
micromamba env create -f environment.yml
micromamba activate fhi

# Install dependencies (Option B: venv)
python3.13 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt -r requirements-dev.txt

# Run development server
./scripts/run_local.sh

# Run all tests via tox
tox

# Run specific test suites
tox -e py313-django52-sync       # Synchronous tests
tox -e py313-django52-async      # Async tests (parallelized)
tox -e py313-django52-sync-actor # Ray actor tests

# Run single test file
python manage.py run_test --test-file tests/async/test_appeal_file_view.py

# Code formatting
black --check fighthealthinsurance fhi_user
```

</details>
