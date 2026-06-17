---
name: telepresenceio__telepresence
source: https://github.com/telepresenceio/telepresence/blob/aed4a6b98858cb8be7f4f3fa20c66343e455e986/CLAUDE.md
repo: telepresenceio/telepresence
kind: claude-md
stars: 7230
last_pushed: 2026-06-15T04:25:39Z
license: apache-2.0
score: 9
domains: [cli-tools, kubernetes]
tags: [build-systems, git-workflow, integration-testing]
curated: 2026-06-15
curated_by: config-scout
---

# telepresenceio/telepresence — claude-md

**Why it's worth keeping:** Includes high-precision instructions for Git hygiene (signing/autosquashing) and explains subtle nuances in test environment configuration precedence. This prevents an AI from making common procedural errors that would fail CI/CD pipelines.

**Summary:** Provides exhaustive technical guidance for building, testing, and contributing to the project, including complex environment requirements. It covers specific command-line workflows and architectural breakdowns.

**Source credibility:** Very high; Telepresence is a popular, actively maintained Kubernetes tool with over 7k stars.

**Recency:** Current; the repository was updated within the last month and follows modern development patterns.

**Source:** [telepresenceio/telepresence/CLAUDE.md](https://github.com/telepresenceio/telepresence/blob/aed4a6b98858cb8be7f4f3fa20c66343e455e986/CLAUDE.md) · 7230★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance for contributors and AI assistants working with this repository.

## Project Overview

Telepresence is a Kubernetes development tool that enables fast local development by connecting your local workstation to a Kubernetes cluster. It allows developers to run services locally while accessing cluster resources and intercepting traffic from the cluster to their local machine.

## Git Workflow

- Never commit directly to the `release/v2` branch. Always create a feature branch with a name following the pattern `username/topic` (e.g., `thallgren/fix-dns-resolution`).
- All commits must be signed and signed-off (`git commit -s -S`).
- Limit commit message subjects to 72 characters. Do not wrap subjects;
  rewrite them shorter instead. Wrap commit message body lines at 72
  characters by default unless preserving exact external text requires a
  longer line.
- **Always run `make lint` and fix every reported issue before pushing.** This is non-negotiable — CI runs the same linters and a push with lint errors wastes a CI cycle. If `make lint` finds problems, fix them in the appropriate commit (use `git commit --fixup=<sha>` followed by `GIT_SEQUENCE_E
```

</details>
