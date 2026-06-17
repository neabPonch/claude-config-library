---
name: MnO2__logq
source: https://github.com/MnO2/logq/blob/2a5672cf99baf12f37d8168e7a0ec2e74969ae1a/CLAUDE.md
repo: MnO2/logq
kind: claude-md
stars: 46
last_pushed: 2026-04-09T17:00:07Z
license: apache-2.0
score: 8
domains: [cli-tools, systems-programming, rust]
tags: [roadmap, architectural-constraints, test-driven]
curated: 2026-06-14
curated_by: config-scout
---

# MnO2/logq — claude-md

**Why it's worth keeping:** The 'Out of Scope' section prevents agentic over-engineering, while the 'Test Oracle' provides clear ground truth instructions for verification.

**Summary:** Provides a structured roadmap, architectural hierarchy, and strict scope boundaries for building a complex system in phases.

**Source credibility:** Active niche Rust project with recent maintenance.

**Recency:** Highly relevant; utilizes modern test-driven development and phased execution patterns ideal for Claude Code.

**Source:** [MnO2/logq/CLAUDE.md](https://github.com/MnO2/logq/blob/2a5672cf99baf12f37d8168e7a0ec2e74969ae1a/CLAUDE.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# logq — PartiQL Query Engine for Server Logs

## Project Overview
logq is a Rust CLI tool implementing PartiQL to query server log files (ELB, ALB, S3, Squid, JSONL). The goal is full PartiQL spec compliance (with pragmatic exclusions) using a bottom-up phased approach.

## Architecture
- **Parser** (`src/syntax/`): nom-based parser producing AST nodes
- **Logical Planner** (`src/logical/`): AST → logical plan tree
- **Physical Executor** (`src/execution/`): Stream-based pull execution with `RecordStream` trait
- **Common Types** (`src/common/`): `Value` enum, type definitions shared across layers

## Implementation Plan
See `docs/plans/2026-04-04-partiql-completion-design-final.md` for the full design.

Phases:
- **Phase 0**: Code cleanup (case-sensitivity, failure→anyhow, dedup, bug fixes)
- **Phase 1**: Foundation (NULL/MISSING propagation, float arithmetic, type coercion, IS NULL/MISSING, ordering, multi-branch CASE WHEN, parse_logic refactor)
- **Phase 2**: Expressions (LIKE, BETWEEN, IN, CAST, ||, COALESCE/NULLIF, string functions, date_part)
- **Phase 3**: Clauses (SELECT VALUE, DISTINCT, path wildcards, JOINs, LATERAL, subqueries)
- **Phase 4**: Set operations (UNION/INTER
```

</details>
