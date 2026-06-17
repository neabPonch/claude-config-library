---
name: nats-io__nats.py
source: https://github.com/nats-io/nats.py/blob/ceb803feb2fbd8f6f2931231be82e80cf48dee67/CLAUDE.md
repo: nats-io/nats.py
kind: claude-md
stars: 1230
last_pushed: 2026-06-12T13:13:22Z
license: apache-2.0
score: 9
domains: [backend, systems-programming, python]
tags: [multi-package, workspace, migration-guide, uv, python]
curated: 2026-06-15
curated_by: config-scout
---

# nats-io/nats.py — claude-md

**Why it's worth keeping:** The explicit distinction between 'Legacy' and 'Modern' coding patterns/testing strategies is vital for large migrations; it provides precise command nuances for specific sub-packages.

**Summary:** A comprehensive guide for a complex multi-package Python workspace managed via uv, distinguishing between legacy and modern implementation paradigms.

**Source credibility:** High; maintained by the NATS organization with high star count and active development.

**Recency:** 

**Source:** [nats-io/nats.py/CLAUDE.md](https://github.com/nats-io/nats.py/blob/ceb803feb2fbd8f6f2931231be82e80cf48dee67/CLAUDE.md) · 1230★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Async Python client and tooling for the [NATS](https://nats.io) messaging system. This is a **uv workspace** with four packages sharing the `nats` namespace.

## Workspace Packages

| Package | Directory | PyPI name | Python | Status |
|---------|-----------|-----------|--------|--------|
| nats-py (legacy client) | `nats/` | `nats-py` | >=3.7 | Production |
| nats-core (modern client) | `nats-core/` | `nats-core` | >=3.13 | In development |
| nats-jetstream | `nats-jetstream/` | `nats-jetstream` | >=3.11 | In development |
| nats-server (test helper) | `nats-server/` | `nats-server` | >=3.11 | Production |

Namespace packaging: `nats-py` provides `nats`, `nats.aio`, `nats.js`, `nats.micro`; `nats-core` provides `nats.client`; `nats-jetstream` provides `nats.jetstream`; `nats-server` provides `nats.server`.

## Prerequisites

- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager
- `nats-server` binary in PATH ([install](https://docs.nats.io/running-a-nats-service/introduction/installation)) -- required for tests

## Build / Dev Commands

```bash
# Install all workspace dependencies
uv sync

# Run all tests (uses nats/tests by default, see [too
```

</details>
