---
name: starlake-ai__starlake__claude
source: https://github.com/starlake-ai/starlake/blob/59695ea6bd1981c589a4cf35702aebf68638547d/src/main/resources/templates/bootstrap/samples/sample-project/CLAUDE.md
repo: starlake-ai/starlake
kind: claude-md
stars: 204
last_pushed: 2026-06-15T06:27:34Z
license: apache-2.0
score: 9
domains: [data-engineering, cli-tools, data-pipelines]
tags: [cli, sql, orchestration, etl]
curated: 2026-06-15
curated_by: config-scout
---

# starlake-ai/starlake — claude-md

**Why it's worth keeping:** Includes critical operational nuances like silent exit behaviors, logging instructions, and platform-specific (Windows vs Unix) CLI differences. The visual DAG/flow diagram is excellent for helping an LLM understand data lineage.

**Summary:** Provides a highly actionable manual for the Starlake CLI and its data pipeline architecture. It defines command syntax, environmental variables, and structural hierarchies.

**Source credibility:** High; the file reflects a well-organized, professional tool documentation style used in active development.

**Recency:** Current; includes modern data stack patterns like DuckDB and specific instructions for Claude Code.

**Source:** [starlake-ai/starlake/src/main/resources/templates/bootstrap/samples/sample-project/CLAUDE.md](https://github.com/starlake-ai/starlake/blob/59695ea6bd1981c589a4cf35702aebf68638547d/src/main/resources/templates/bootstrap/samples/sample-project/CLAUDE.md) · 204★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Starlake** data pipeline project ("StarBake") — a sample bakery analytics system demonstrating data ingestion, transformation, and KPI computation. The default engine is **DuckDB** (configurable via environment files).

## Starlake CLI

Before running any `starlake` command, verify the CLI is available in the PATH by running `starlake --version`. If not found, ask the user for the path to the starlake executable. On Windows, the command is `starlake.cmd` instead of `starlake`.

The CLI is silent by default — exit code 0 with empty stdout means success, not a no-op. To see execution logs (SQL run, write strategies, audit inserts), prefix the command with `SL_LOG_LEVEL=info`.

## Key Commands

```bash
# Validate project configuration
starlake validate

# Load source data (CSV/JSON) into the warehouse
# Always specify --domains, --tables, and --files explicitly
starlake load --domains starbake --tables customers --files "${SL_ROOT}/datasets/incoming/starbake/customers.csv"
starlake load --domains starbake --tables orders --files "${SL_RO
```

</details>
