---
name: rero__rero-ils
source: https://github.com/rero/rero-ils/blob/388aae0c6b725aceb79b65bde7d1692ef7cb3328/CLAUDE.md
repo: rero/rero-ils
kind: claude-md
stars: 86
last_pushed: 2026-06-15T20:47:18Z
license: agpl-3.0
score: 9
domains: [backend-api, python]
tags: [architectural-mapping, behavioral-constraints, minimalism]
curated: 2026-06-16
curated_by: config-scout
---

# rero/rero-ils — claude-md

**Why it's worth keeping:** The 'Module Structure' breakdown is a masterclass in providing architectural context, and the 'Surgical Changes' rule effectively minimizes unnecessary diff noise.

**Summary:** This guide provides a deep structural map of the project's module patterns and strict behavioral constraints to prevent AI over-engineering.

**Source credibility:** Highly credible; an active, specialized library system with recent updates.

**Recency:** Very current; includes modern toolchain mentions like 'uv'.

**Source:** [rero/rero-ils/CLAUDE.md](https://github.com/rero/rero-ils/blob/388aae0c6b725aceb79b65bde7d1692ef7cb3328/CLAUDE.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RERO ILS Claude guide

## Overview

rero-ils is the Python/Flask backend of the RERO ILS Integrated Library System (ILS). Some frontend elements are defined in this project as HTML/Jinja templates, the rest is a separate Angular project (rero-ils-ui) based on (ng-core).

**Stack**: Python 3.14, Flask (Invenio), PostgreSQL, Elasticsearch 7, Celery, RabbitMQ, Redis
**Package manager**: `uv` with `poethepoet` for task running

## Commands

During development, all commands are run through uv's virtual env with `uv run`.

### Linting and formatting

**IMPORTANT:** After editing files, make sure that there are no errors in the formatting and linting.

```bash
uv run poe lint     # ruff check rero_ils tests
uv run poe format   # ruff format rero_ils tests
```

### Setup (done by humans)

Human developers will run the required containers, the app setup and the servers on their own terms.

## Architecture

### Module Structure

All business logic lives in `rero_ils/modules/`. Each module follows a consistent pattern:

```text
rero_ils/modules/<module_name>/
├── api.py            # Record class + Search class (core business logic)
├── models.py         # SQLAlchemy model + Identifier + Met
```

</details>
