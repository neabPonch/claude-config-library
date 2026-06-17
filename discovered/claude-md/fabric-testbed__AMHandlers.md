---
name: fabric-testbed__AMHandlers
source: https://github.com/fabric-testbed/AMHandlers/blob/1bacb8f0202edfbc2d7471deda2fbe1ed1352a79/CLAUDE.md
repo: fabric-testbed/AMHandlers
kind: claude-md
stars: 4
last_pushed: 2026-05-20T18:43:36Z
license: mit
score: 9
domains: [devops, infrastructure-as-code, backend, automation]
tags: [ansible, python, provisioning, handler-pattern]
curated: 2026-06-15
curated_by: config-scout
---

# fabric-testbed/AMHandlers — claude-md

**Why it's worth keeping:** The architecture table provides an immediate mental map for the AI, and the explicit mention of `test_mode = True` is a critical instruction to prevent destructive infrastructure calls during testing.

**Summary:** Provides high-density structural context mapping specific handlers to their files and functional purposes. It explicitly defines the provisioning logic flow and configuration patterns.

**Source credibility:** Strong; high-quality technical documentation for specialized infrastructure/research code with recent maintenance.

**Recency:** Very current; references Python 3.12 and modern packaging via flit.

**Source:** [fabric-testbed/AMHandlers/CLAUDE.md](https://github.com/fabric-testbed/AMHandlers/blob/1bacb8f0202edfbc2d7471deda2fbe1ed1352a79/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**fabric_am_handlers** — Resource handlers for FABRIC testbed Aggregate Managers (AMs). Each handler manages substrate-specific provisioning (VMs, networks, switches, storage, PCI devices) by executing Ansible playbooks and SSH commands against site infrastructure.

Part of the [FABRIC Control Framework](https://github.com/fabric-testbed/ControlFramework). Version tracked in `fabric_am/__init__.py`.

## Build & Install

```bash
# Uses flit as build backend
pip install flit
flit install            # install in development mode
flit build              # build distribution
```

## Testing

```bash
# Unit tests (pytest)
pip install pytest
pytest fabric_am/test/

# Run a single test file
pytest fabric_am/test/test_vm_handler.py

# Integration playbook tests (requires infrastructure access)
python test_playbooks.py
```

Test files use `handler.test_mode = True` to bypass actual infrastructure calls.

## Architecture

### Handler Pattern

All handlers inherit from `HandlerBase` (from `fabric_cf`) and implement:
- `create()` — provision a resource
- `del
```

</details>
