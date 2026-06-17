---
name: abh__ntppool
source: https://github.com/abh/ntppool/blob/cc4a6fe379e07c8c88b481982f652bb2e29b02c7/CLAUDE.md
repo: abh/ntppool
kind: claude-md
stars: 250
last_pushed: 2026-06-14T07:32:09Z
license: other
score: 9
domains: [web-frontend, security, devops]
tags: [git-workflow, csp-compliance, tool-orchestration, perl]
curated: 2026-06-14
curated_by: config-scout
---

# abh/ntppool — claude-md

**Why it's worth keeping:** The instructions for parallelizing tool calls and the robust Git commit workflow using HEREDOCs are highly advanced, transferable patterns for agentic coding.

**Summary:** This file combines critical architectural constraints (strict CSP rules) with hyper-specific operational protocols for agent tool usage and git workflows.

**Source credibility:** High; comes from an established, active open-source project (NTP Pool).

**Recency:** Current; specifically optimized for modern agentic capabilities like parallel tool execution.

**Source:** [abh/ntppool/CLAUDE.md](https://github.com/abh/ntppool/blob/cc4a6fe379e07c8c88b481982f652bb2e29b02c7/CLAUDE.md) · 250★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

The NTP Pool Project is a website frontend for managing a global cluster of NTP time servers. It's written in Perl using Template Toolkit templates and the internal "Combust" web framework. The system runs in Kubernetes in production and has many dependencies.

## Technology Stack

- **Language**: Perl (latest released version)
- **Web Framework**: Internal "Combust" framework
- **Templates**: Template Toolkit
- **Database**: MySQL (accessed via internal API service)
- **Database ORM**: Rose::DB
- **Containerization**: Docker/Kubernetes
- **Build System**: ExtUtils::MakeMaker (Makefile.PL)

## Development Commands

### Building and Testing
- `make` - Build the project
- `make test` - Run tests (files in `t/*.t`)
- `make clean` - Clean build artifacts

### Code Formatting (Required Before Commits)
- `perltidy` - Format Perl code (run before committing)

### Docker Development
- Uses `Dockerfile.dev` during development
- Built into Docker containers, executed in Kubernetes

## LLM Coding Agent Guidelines

### CRITICAL: Content Security Policy (CSP) Complia
```

</details>
