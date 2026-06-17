---
name: cockroachdb__cockroach__claude
source: https://github.com/cockroachdb/cockroach/blob/f0bf32430c4960bfdad6d867e6df0e67079aeee1/pkg/sql/logictest/CLAUDE.md
repo: cockroachdb/cockroach
kind: claude-md
stars: 32206
last_pushed: 2026-06-11T22:40:23Z
license: other
score: 9
domains: [database, testing-framework, distributed-systems]
tags: [sql, dsl, e2e-testing]
curated: 2026-06-15
curated_by: config-scout
---

# cockroachdb/cockroach — claude-md

**Why it's worth keeping:** Provides precise grammar rules for a custom SQL-based DSL (statements, queries, variables) and actionable patterns for iterative test development using '_tmp' files.

**Summary:** Technical specification for the LogicTest SQL testing framework, covering DSL syntax, CLI commands, and configuration profiles.

**Source credibility:** High; derived from the official CockroachDB repository, a major distributed database project.

**Recency:** Current; includes recent versioning and configuration details relevant to modern workflows.

**Source:** [cockroachdb/cockroach/pkg/sql/logictest/CLAUDE.md](https://github.com/cockroachdb/cockroach/blob/f0bf32430c4960bfdad6d867e6df0e67079aeee1/pkg/sql/logictest/CLAUDE.md) · 32206★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# LogicTest Framework

This directory contains CockroachDB's primary end-to-end SQL testing infrastructure.
All test files (including enterprise/CCL features) are in `testdata/logic_test/`.

## Running Tests

Running with `--config=local` is usually the quickest way to run a test.

```bash
# Run all tests with default configs
./dev testlogic base

# Run specific test file(s)
./dev testlogic base --config=local --files='fk'      # Files matching 'fk'
./dev testlogic base --config=local --files='_tmp'    # The _tmp file (for iteration)
./dev testlogic base --files='(fk|grant)'             # Multiple patterns, all default configs

# Run with specific config
./dev testlogic base --config=local
./dev testlogic base --config=fakedist

# Useful flags
./dev testlogic base --files='_tmp' -v              # Verbose output
./dev testlogic base --files='_tmp' --show-sql      # Print SQL as it runs
./dev testlogic base --files='_tmp' --rewrite       # Update expected results
```

## Adding a Test File

Use an existing test file if there already is a good place to add a test.

If you do add a new test file, then regenerate Bazel build files:

```bash
./dev generate bazel
```

## Test File Syntax
```

</details>
