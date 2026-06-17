---
name: prashantkul__causal-armor
source: https://github.com/prashantkul/causal-armor/blob/97442c6ee7dec1b803828c81ec4c497b0d91f5cc/CLAUDE.md
repo: prashantkul/causal-armor
kind: claude-md
stars: 8
last_pushed: 2026-02-23T22:39:57Z
license: mit
score: 9
domains: [python, security, ai-safety]
tags: [backend, strict-typing, ruff, pytest]
curated: 2026-06-15
curated_by: config-scout
---

# prashantkul/causal-armor — claude-md

**Why it's worth keeping:** The inclusion of an explicit directory-to-purpose map, specific linter rule warnings (e.g., RUF005), and high-level 'Architecture principles' prevents the LLM from suggesting incompatible patterns.

**Summary:** A high-rigor configuration for a published Python library that emphasizes CI compliance and structural integrity. It provides clear constraints on coding patterns to prevent architectural drift.

**Source credibility:** Solid; a niche but published research implementation with active maintenance/recent commits.

**Recency:** Very current; uses modern Python 3.11+ standards and contemporary tooling like Ruff.

**Source:** [prashantkul/causal-armor/CLAUDE.md](https://github.com/prashantkul/causal-armor/blob/97442c6ee7dec1b803828c81ec4c497b0d91f5cc/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — CausalArmor

## Important: Open source library

This is a published open source library on PyPI. Exercise extra caution:

- **Do not introduce errors** — always run the full check suite before committing
- **Always run `make lint` and `make format` before committing** (or equivalently `.venv/bin/ruff check src/ tests/` and `.venv/bin/ruff format src/ tests/`)
- **Run tests** (`make test`) to verify nothing is broken
- Prefer `make check` (lint + typecheck + test) for a complete pre-commit validation
- Be careful with public API changes — they affect downstream users

## Project overview

CausalArmor is a Python library implementing indirect prompt injection guardrails via causal attribution. It follows a two-phase architecture (scoring + regeneration) based on Algorithm 2 from [arXiv:2602.07918](https://arxiv.org/abs/2602.07918).

**Core pipeline**: `build_structured_context` → `compute_attribution` → `detect_dominant_spans` → `defend` (sanitize + mask CoT + regenerate)

**Entry point for users**: `CausalArmorMiddleware.guard()` orchestrates the full pipeline.

## Repository layout

```
src/causal_armor/
  __init__.py          # Public API re-exports
  types.py
```

</details>
