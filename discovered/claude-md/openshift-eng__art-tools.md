---
name: openshift-eng__art-tools
source: https://github.com/openshift-eng/art-tools/blob/3b263c10f8a0220af696eb31935b341b96a46303/CLAUDE.md
repo: openshift-eng/art-tools
kind: claude-md
stars: 12
last_pushed: 2026-06-12T15:52:40Z
license: apache-2.0
score: 9
domains: [cli-tools, devops, python]
tags: [multi-package, architecture-driven, workflow-rules]
curated: 2026-06-15
curated_by: config-scout
---

# openshift-eng/art-tools — claude-md

**Why it's worth keeping:** Uses highly specific Git remote/branch constraints to prevent errors and details the 'Runtime' pattern to help Claude understand object orchestration across packages.

**Summary:** Provides a deep structural map of a multi-package Python ecosystem, covering setup, testing, and specific architectural patterns.

**Source credibility:** High; maintained by an active OpenShift engineering team with clear, production-grade documentation.

**Recency:** Current; utilizes modern Python tooling like uv and targeting Python 3.11.

**Source:** [openshift-eng/art-tools/CLAUDE.md](https://github.com/openshift-eng/art-tools/blob/3b263c10f8a0220af696eb31935b341b96a46303/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

If the file `.claude/CLAUDE.md` exists, read it. If instructions contradict (for example for what to run with test or run commands), `.claude/CLAUDE.md` takes precedence over this file.

## Overview

This is **art-tools**, a collection of Release tools for managing OpenShift Container Platform (OCP) releases. The repository contains multiple Python packages that work together to automate the OCP release process.

### Core Components

- **doozer** (`./doozer/`) - CLI tool for managing builds via OSBS/Brew (RPMs and container images)
- **elliott** (`./elliott/`) - CLI tool for managing release advisories, errata, and bugs
- **pyartcd** (`./pyartcd/`) - Pipeline code for automated release pipelines (entry point: `artcd`)
- **artcommon** (`./artcommon/`) - Common package used by doozer, elliott, and pyartcd
- **ocp-build-data-validator** (`./ocp-build-data-validator/`) - Schema validator for ocp-build-data

## Development Setup

### Environment Setup

Python 3.11 is the target version (minimum Python 3.11 required). Use `uv` for package management:

```bash
# Create virt
```

</details>
