---
name: sethlaw__sputr
source: https://github.com/sethlaw/sputr/blob/7a1cf4cc6b1e2571c6ca4ed1c4bcf8aee06c65b0/CLAUDE.md
repo: sethlaw/sputr
kind: claude-md
stars: 86
last_pushed: 2026-02-18T02:45:33Z
license: gpl-3.0
score: 8
domains: [security, cli-tools, python]
tags: [architecture-map, command-reference]
curated: 2026-06-14
curated_by: config-scout
---

# sethlaw/sputr — claude-md

**Why it's worth keeping:** It documents non-obvious business logic like the 5-char binary string test selection and the specific lifecycle of the Report object through the test chain.

**Summary:** Provides a highly structured technical map of the security testing framework, covering CLI usage, architectural hierarchy, and internal logic flows.

**Source credibility:** A specialized security tool with moderate star count and recent activity.

**Recency:** 

**Source:** [sethlaw/sputr/CLAUDE.md](https://github.com/sethlaw/sputr/blob/7a1cf4cc6b1e2571c6ca4ed1c4bcf8aee06c65b0/CLAUDE.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

SPUTR (Security Payload Unit Test Repository) is a Python 3 security testing framework that automates penetration testing of web applications. It sends generated payloads against configured endpoints and checks for vulnerabilities: SQLi, XSS, IDOR, CSRF, and Missing Function Level Access Control (MFLAC).

## Commands

```bash
# Install dependencies
pip install -r requirements.txt

# Run standard tests against a target app
python3 sputr.py --config config.json --test

# Run raw HTTP request tests
python3 sputr.py --config config.json --raw

# CSRF-only testing
python3 sputr.py --config config.json --testcsrf

# Generate a config template
python3 sputr.py --generate --apptype django --appdir /path/to/app --conf_output config.json

# Verbose output
python3 sputr.py --config config.json --test --verbose
```

There is no linting, type checking, or unit test suite configured for the framework itself.

## Architecture

**Entry point**: `sputr.py` — parses CLI args, loads config, orchestrates test execution.

**Two test modes** with separate base classes
```

</details>
