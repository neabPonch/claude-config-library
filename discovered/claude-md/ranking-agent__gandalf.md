---
name: ranking-agent__gandalf
source: https://github.com/ranking-agent/gandalf/blob/a39fe7ef8e203cd285bf0d991e16e882d8095937/CLAUDE.MD
repo: ranking-agent/gandalf
kind: claude-md
stars: 2
last_pushed: 2026-06-09T12:45:51Z
license: mit
score: 9
domains: [data-science, cli-tools, backend]
tags: [python, graph-algorithms, testing-guidelines]
curated: 2026-06-15
curated_by: config-scout
---

# ranking-agent/gandalf — claude-md

**Why it's worth keeping:** The 'Best practice' section provides excellent coding philosophy (doctests over unittest, fail fast), while the installation notes solve specific environment/dependency bugs before they happen.

**Summary:** A highly detailed guide for a high-performance graph analysis library that includes specific environmental caveats and architectural patterns.

**Source credibility:** Professional documentation for a specialized bioinformatics tool with recent activity.

**Recency:** Very current; accounts for modern Python dependency and setuptools nuances.

**Source:** [ranking-agent/gandalf/CLAUDE.MD](https://github.com/ranking-agent/gandalf/blob/a39fe7ef8e203cd285bf0d991e16e882d8095937/CLAUDE.MD) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD

## Project Overview

GANDALF (Graph Analysis Navigator for Discovery And Link Finding) is a Python library for fast 3-hop path finding in large biomedical knowledge graphs. It's designed for the Translator project to efficiently query biological relationships (e.g., drug → protein → disease).

## Tech Stack

- **Python 3.8+** (supports 3.8-3.12)
- **FastAPI** - REST API server
- **NumPy** - Sparse matrix operations
- **BMT** (Biolink Model Toolkit) - Biolink ontology handling
- **pytest** - Testing framework
- **black** - Code formatting

## Installation

**Important:** An up-to-date `setuptools` (>=69) is required before installing
dependencies.  BMT transitively depends on legacy packages (`stringcase`,
`pytest-logging`) whose `setup.py` installs fail with older setuptools due to a
`distutils` `install_layout` bug.  Always upgrade setuptools first.

```bash
pip install -U pip setuptools wheel
pip install -e ".[dev]"
```

## Quick Commands

```bash
# Build graph from JSONL
gandalf-build --edges data/edges.jsonl --nodes data/nodes.jsonl --output graph_mmap/

# Query paths
gandalf-query --graph graph_mmap/ --start "CHEBI:45783" --end "MONDO:0004979"

# Diagnose path exp
```

</details>
