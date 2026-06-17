---
name: VV1NN__APT_Attribution_Thesis
source: https://github.com/VV1NN/APT_Attribution_Thesis/blob/58b3c4373619f0731abfddc1ff68ba0534a43e7c/CLAUDE.md
repo: VV1NN/APT_Attribution_Thesis
kind: claude-md
stars: 0
last_pushed: 2026-04-06T16:02:53Z
license: unknown
score: 9
domains: [security, data-pipeline, graph-databases]
tags: [knowledge-graph, api-integration, state-tracking, cybersecurity]
curated: 2026-06-14
curated_by: config-scout
---

# VV1NN/APT_Attribution_Thesis — claude-md

**Why it's worth keeping:** The 'API Constraints' section provides critical rate-limit/retry logic to prevent runtime errors, and the 'Current Progress' section offers high-fidelity context regarding data completeness.

**Summary:** A highly detailed technical manual for a cybersecurity data pipeline that includes rigorous API constraint documentation and real-time state tracking via progress tables.

**Source credibility:** Low social proof (0 stars), but appears to be a highly structured academic research project.

**Recency:** Very recent; uses modern tooling like `uv` and reflects current development status.

**Source:** [VV1NN/APT_Attribution_Thesis/CLAUDE.md](https://github.com/VV1NN/APT_Attribution_Thesis/blob/58b3c4373619f0731abfddc1ff68ba0534a43e7c/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

APT (Advanced Persistent Threat) knowledge graph construction pipeline for a master's thesis. The system extracts IoCs (Indicators of Compromise) from CTI reports, enriches them via VirusTotal API, builds two-layer knowledge graphs per APT group, and merges them into a unified queryable database.

## Setup & Common Commands

**Package manager:** `uv` (Python 3.12, specified in `.python-version`)
> PyTorch CUDA index 僅在 Linux 啟用（`marker = "sys_platform == 'linux'"`），macOS 使用預設 PyPI。

```bash
uv sync                              # Install/update dependencies
```

**Pipeline scripts (all run via `uv run python`):**

```bash
# IoC cleaning
uv run python ioc_clean_code/clean_iocs_v2.py

# VT metadata enrichment
uv run python scripts/fetch_vt_metadata.py --org APT18

# VT relationship discovery
uv run python scripts/fetch_vt_relationships.py --org APT18

# Build knowledge graph (Phase 1 + 2)
uv run python scripts/build_knowledge_graph.py --org APT18
uv run python scripts/build_knowledge_graph.py --org APT18 --skip-query    # skip VT API calls
uv run py
```

</details>
