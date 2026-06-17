---
name: FreedomIntelligence__OpenClaw-Medical-Skills__skill
source: https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills/blob/2aa60d4d86d3a028358f4505684a24efe745a8ea/skills/geniml/SKILL.md
repo: FreedomIntelligence/OpenClaw-Medical-Skills
kind: skill
stars: 2704
last_pushed: 2026-03-27T02:21:01Z
license: unknown
score: 8
domains: [bioinformatics, machine-learning, genomics]
tags: [genomics, embeddings, scATAC-seq, ml-pipelines]
curated: 2026-06-16
curated_by: config-scout
---

# FreedomIntelligence/OpenClaw-Medical-Skills — skill

**Why it's worth keeping:** Provides full end-to-end code workflows, precise CLI commands, and explicit decision logic that allows an agent to perform complex bioinformatics tasks autonomously.

**Summary:** A technical specification for the geniml library used for genomic interval machine learning and embedding generation.

**Source credibility:** High; part of a specialized medical AI library with significant community traction (2.7k stars).

**Recency:** Current; utilizes modern Python tooling like `uv` for dependency management.

**Source:** [FreedomIntelligence/OpenClaw-Medical-Skills/skills/geniml/SKILL.md](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills/blob/2aa60d4d86d3a028358f4505684a24efe745a8ea/skills/geniml/SKILL.md) · 2704★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: geniml
description: This skill should be used when working with genomic interval data (BED files) for machine learning tasks. Use for training region embeddings (Region2Vec, BEDspace), single-cell ATAC-seq analysis (scEmbed), building consensus peaks (universes), or any ML-based analysis of genomic regions. Applies to BED file collections, scATAC-seq data, chromatin accessibility datasets, and region-based genomic feature learning.
---

# Geniml: Genomic Interval Machine Learning

## Overview

Geniml is a Python package for building machine learning models on genomic interval data from BED files. It provides unsupervised methods for learning embeddings of genomic regions, single cells, and metadata labels, enabling similarity searches, clustering, and downstream ML tasks.

## Installation

Install geniml using uv:

```bash
uv uv pip install geniml
```

For ML dependencies (PyTorch, etc.):

```bash
uv uv pip install 'geniml[ml]'
```

Development version from GitHub:

```bash
uv uv pip install git+https://github.com/databio/geniml.git
```

## Core Capabilities

Geniml provides five primary capabilities, each detailed in dedicated reference files:

### 1. Region2Vec: Genomic
```

</details>
