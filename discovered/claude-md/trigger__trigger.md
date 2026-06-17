---
name: trigger__trigger
source: https://github.com/trigger/trigger/blob/48cc719c5c2a754b088143532659d0515b3e9c3d/CLAUDE.md
repo: trigger/trigger
kind: claude-md
stars: 557
last_pushed: 2026-06-03T22:45:14Z
license: other
score: 9
domains: [cli-tools, network-automation, backend]
tags: [python, architecture-heavy, devops]
curated: 2026-06-14
curated_by: config-scout
---

# trigger/trigger — claude-md

**Why it's worth keeping:** The inclusion of 'Data Flow' diagrams and a structured 'Core Component Layers' section is a masterclass in helping an AI understand system-wide side effects and dependencies. The explicit list of test environment variables is also a high-value detail for debugging.

**Summary:** This file provides deep architectural insights, including data flow diagrams and component-layer breakdowns. It also includes highly specific development workflows for testing, linting, and installation.

**Source credibility:** High; it is a mature, enterprise-grade network automation tool with significant GitHub history.

**Recency:** Current; the documentation includes modern Python tooling like uv and ruff.

**Source:** [trigger/trigger/CLAUDE.md](https://github.com/trigger/trigger/blob/48cc719c5c2a754b088143532659d0515b3e9c3d/CLAUDE.md) · 557★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Trigger is a mature network automation toolkit written in Python for managing network devices at scale. Originally developed by AOL's Network Security team in 2006, it provides asynchronous command execution, ACL parsing/management, and metadata-driven device interaction across multiple vendor platforms (Cisco IOS/NX-OS/ASA, Juniper Junos/ScreenOS, Force10 FTOS, Arista, etc.).

**Key characteristics:**
- Python 3.10-3.11 codebase (v2.0.0+; Python 2.7 support ended with v1.6.0)
- Twisted-based asynchronous I/O framework
- Enterprise-scale network automation (hundreds to thousands of devices)
- Grammar-based ACL parsing and format conversion
- Redis-backed ACL database and deployment queue

## Development Commands

### Running Tests

**Unit tests:**
```bash
# Run all unit tests
pytest

# Run with verbose output
pytest -vv

# Run specific test file
pytest tests/test_acl.py

# Run with coverage
pytest --cov=trigger tests/
```

**Test environment variables** (automatically set by conftest.py):
- `TRIGGER_SETTINGS`: Path to test settings.py
- `NETDEVIC
```

</details>
