---
name: mriffle__parquet-to-tsv
source: https://github.com/mriffle/parquet-to-tsv/blob/d330d802561e43dbc8187b7e68b076a2ecd50d63/CLAUDE.md
repo: mriffle/parquet-to-tsv
kind: claude-md
stars: 0
last_pushed: 2026-05-06T19:10:39Z
license: apache-2.0
score: 9
domains: [cli-tools, data-engineering]
tags: [python, cli, streaming, invariants]
curated: 2026-06-14
curated_by: config-scout
---

# mriffle/parquet-to-tsv — claude-md

**Why it's worth keeping:** It defines 'core behaviors' as immutable rules (atomicity, streaming) and provides exact execution sequences to prevent the AI from suggesting refactors that break logic flow. It also solves environment ambiguity by specifying absolute paths to venv tools.

**Summary:** A high-density instruction set that focuses on behavioral invariants and architectural order of operations for a mission-critical CLI tool.

**Source credibility:** Single-author repo with highly professional, rigorous documentation style.

**Recency:** Current; adheres to modern Python standards like PEP 668 and structured tool execution.

**Source:** [mriffle/parquet-to-tsv/CLAUDE.md](https://github.com/mriffle/parquet-to-tsv/blob/d330d802561e43dbc8187b7e68b076a2ecd50d63/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this project is

A small, single-purpose CLI that converts a Parquet file to a TSV
(tab-separated values) file. It is built for use as a step inside
computational workflows (Snakemake, Nextflow, plain shell pipelines),
where correctness, predictable failure modes, and bounded memory matter
more than feature breadth.

Core behaviours that callers (and any change you make) must preserve:

- **Streaming.** Rows flow from parquet in batches via
  `pyarrow.parquet.ParquetFile.iter_batches`. The full table is never
  loaded into memory.
- **Atomic output.** Bytes are written to a sibling `<output>.tmp`,
  `fsync`'d, validated, then `Path.replace()`'d into place. Any failure
  unlinks the temp file and leaves any pre-existing output untouched.
- **Row-count verification.** The number of rows actually written is
  compared to `pf.metadata.num_rows` before the rename. A mismatch raises
  `RowCountMismatchError`.
- **Fail-loud.** Tab/newline/CR inside string cells, unsupported column
  types (binary, list, struct, map, …), and bad arguments all abort
  *before* any byt
```

</details>
