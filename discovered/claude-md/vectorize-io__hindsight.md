---
name: vectorize-io__hindsight
source: https://github.com/vectorize-io/hindsight/blob/42e72601f420e9c4a9070e82a401f4efe311afae/CLAUDE.md
repo: vectorize-io/hindsight
kind: claude-md
stars: 16397
last_pushed: 2026-06-14T02:33:22Z
license: mit
score: 9
domains: [backend-api, ai-agents, monorepo]
tags: [python, devops, database-migrations, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# vectorize-io/hindsight — claude-md

**Why it's worth keeping:** It offers exact CLI commands for all tasks and an essential code template for critical workflows like cross-dialect database migrations, preventing architectural drift.

**Summary:** This file provides exhaustive command sets for a multi-component monorepo, covering API development, UI, benchmarks, and client generation. It includes high-stakes procedural guidance for complex database migrations.

**Source credibility:** Extremely high; the repository is highly popular with 16k+ stars and active development.

**Recency:** Very current, utilizing modern toolchains like uv, ruff, and FastAPI.

**Source:** [vectorize-io/hindsight/CLAUDE.md](https://github.com/vectorize-io/hindsight/blob/42e72601f420e9c4a9070e82a401f4efe311afae/CLAUDE.md) · 16397★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Hindsight is an agent memory system that provides long-term memory for AI agents using biomimetic data structures. Memories are organized as:
- **World facts**: General knowledge ("The sky is blue")
- **Experience facts**: Personal experiences ("I visited Paris in 2023")
- **Mental models**: Consolidated knowledge synthesized from facts ("User prefers functional programming patterns")

## Development Commands

### Local Development (API + UI)
```bash
# Start both API server and control plane UI
./scripts/dev/start.sh
```

### API Server (Python/FastAPI)
```bash
# Start API server only (loads .env automatically)
./scripts/dev/start-api.sh

# Run all tests (parallelized with pytest-xdist)
cd hindsight-api-slim && uv run pytest tests/

# Run specific test file
cd hindsight-api-slim && uv run pytest tests/test_http_api_integration.py -v

# Run single test function
cd hindsight-api-slim && uv run pytest tests/test_retain.py::test_retain_simple -v

# Lint and format
cd hindsight-api-slim && uv run ruff check .
cd hindsight-api-slim && uv run ruff forma
```

</details>
