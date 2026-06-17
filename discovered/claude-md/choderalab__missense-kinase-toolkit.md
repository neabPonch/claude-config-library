---
name: choderalab__missense-kinase-toolkit
source: https://github.com/choderalab/missense-kinase-toolkit/blob/39e4a2285951943f9f1ef24aaf0432dc3528b560/CLAUDE.MD
repo: choderalab/missense-kinase-toolkit
kind: claude-md
stars: 3
last_pushed: 2026-06-12T21:34:38Z
license: mit
score: 9
domains: [bioinformatics, data-science, python-monorepo]
tags: [monorepo, pydantic, dependency-management, scientific-computing]
curated: 2026-06-16
curated_by: config-scout
---

# choderalab/missense-kinase-toolkit — claude-md

**Why it's worth keeping:** The visual dependency chain and the deep semantic explanation of core Pydantic models provide critical context for an AI to understand architectural constraints.

**Summary:** An exceptional guide for a complex Python mono repo that defines how sub-packages interact and how data models are structured.

**Source credibility:** High; active development (0 months ago) and a specialized scientific domain indicate professional-grade documentation.

**Recency:** Very current; provides specific, actionable terminal commands for modern Python environments.

**Source:** [choderalab/missense-kinase-toolkit/CLAUDE.MD](https://github.com/choderalab/missense-kinase-toolkit/blob/39e4a2285951943f9f1ef24aaf0432dc3528b560/CLAUDE.MD) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

`missense-kinase-toolkit` (mkt) is a Python mono repo for integrating kinase data from multiple sources (KLIFS, KinCore, UniProt, cBioPortal, OncoKB, ChEMBL, OpenTargets, HGNC, Pfam, NCBI, ProtVar), modeling kinase schemas with Pydantic, and building ML models for kinase activity prediction. It also includes a Streamlit web application for interactive kinase exploration.

## Mono Repo Structure

All sub-packages reside under `missense_kinase_toolkit/`:

| Sub-package | Pip name | Import namespace | Description |
|---|---|---|---|
| `schema/` | `mkt-schema` | `mkt.schema` | Core Pydantic models (`KinaseInfo`), serialization (json/yaml/toml), constants (KLIFS regions, kinase groups) |
| `databases/` | `mkt-databases` | `mkt.databases` | API clients, web scrapers, data harmonization, plotting, CLI tools |
| `ml/` | `mkt-ml` | `mkt.ml` | PyTorch models (cross-attention, factor), HuggingFace encoders (ChemBERTa, ESM2), W&B tracking |
| `experiments/` | `experiments` | `missense_kinase_toolkit.experiments` | Experimental analysis tools (minimal, poetry
```

</details>
