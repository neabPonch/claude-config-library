---
name: compdemocracy__polis__claude
source: https://github.com/compdemocracy/polis/blob/32ec6fcb940f85e26b86bdda18724150e8c63564/delphi/CLAUDE.md
repo: compdemocracy/polis
kind: claude-md
stars: 1174
last_pushed: 2026-06-11T21:49:27Z
license: agpl-3.0
score: 9
domains: [backend, devops, data-engineering, cli-tools]
tags: [database, docker, debugging, environment-config]
curated: 2026-06-15
curated_by: config-scout
---

# compdemocracy/polis — claude-md

**Why it's worth keeping:** Includes critical 'invariant' warnings about venv symlinks and provides ready-to-use Python one-liners for querying distributed job logs that aren't in stdout.

**Summary:** Provides deep operational intelligence for the Delphi system, including environment gotchas, database inspection templates, and complex log-retrieval scripts.

**Source credibility:** High; comes from a well-maintained, high-star open-source project (Polis).

**Recency:** Current; references modern Python 3.12 and specific local LLM/Ollama integrations.

**Source:** [compdemocracy/polis/delphi/CLAUDE.md](https://github.com/compdemocracy/polis/blob/32ec6fcb940f85e26b86bdda18724150e8c63564/delphi/CLAUDE.md) · 1174★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Delphi System Reference Guide

This document provides comprehensive guidance for working with the Delphi system, including database interactions, environment configuration, Docker services, and the distributed job queue system. It serves as both documentation and a practical reference for day-to-day operations.

## Documentation

**Warning:** Many docs in `docs/` are outdated and should not be trusted. Always verify against the actual code. Start with `docs/PLAN_DISCREPANCY_FIXES.md` (canonical fix plan) and `docs/CLJ-PARITY-FIXES-JOURNAL.md` (session journal) for current Clojure parity work.

## Helpful terminology

zid - conversation id
pid - participant id
tid - comment id

this avoids the confusion of having anything called a "cid", the joke was "conversationzzzz", that's why it's a zid throughout the codebase

## helpful background

this was built in two parts, the pca/kmenas/repness and the umap/narrative, and these are combined in the run_delphi.sh script.

## Local Python Environment

Canonical venv: `delphi/.venv` (Python 3.12). Setup is documented for humans in
[`README.md`](README.md#local-python-development) and
[`docs/QUICK_START.md`](docs/QUICK_START.md#environment-
```

</details>
