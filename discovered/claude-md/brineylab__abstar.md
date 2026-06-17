---
name: brineylab__abstar
source: https://github.com/brineylab/abstar/blob/c0b7c2949d0aac716a32c280ca871512471f591d/CLAUDE.md
repo: brineylab/abstar
kind: claude-md
stars: 44
last_pushed: 2026-03-30T17:05:42Z
license: mit
score: 9
domains: [bioinformatics, cli-tools, data-science]
tags: [biology, sequence-annotation, pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# brineylab/abstar — claude-md

**Why it's worth keeping:** The split between CLI and Python API examples is vital for LLMs; including a text-based 'Data Flow' diagram and module responsibilities provides excellent context for refactoring tasks.

**Summary:** A highly structured guide that covers command-line usage, programmatic API patterns, and detailed architectural flows. It excels at explaining not just what the code does, but how data moves through specific modules.

**Source credibility:** A specialized bioinformatics tool with respectable engagement (44 stars) and recent maintenance.

**Recency:** 

**Source:** [brineylab/abstar/CLAUDE.md](https://github.com/brineylab/abstar/blob/c0b7c2949d0aac716a32c280ca871512471f591d/CLAUDE.md) · 44★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

abstar is a VDJ assignment and antibody/TCR sequence annotation tool. It performs germline gene assignment using MMseqs2 and detailed sequence annotation including mutations, indels, regions (CDR/FWR), and productivity assessment. Scalable from single sequences to billions.

## Common Commands

### Running Tests
```bash
# Run full test suite
pytest

# Run a single test file
pytest abstar/tests/test_regions.py

# Run a specific test
pytest abstar/tests/test_regions.py::test_get_region_sequence_fwr1

# Run with verbose output
pytest -v
```

### Installation
```bash
pip install -e .  # Development install
pip install abstar  # Production install
```

### CLI Usage
```bash
# Annotate sequences
abstar run path/to/sequences.fasta path/to/project_directory

# Build custom germline database
abstar build_germline_database <name> -f <fasta_files> -j <json_files>
```

### Python API
```python
import abstar

# Annotate sequences (returns Sequence objects when no project_path)
sequences = abstar.run("sequences.fasta")

# Annotate with output files
abstar.run(
```

</details>
