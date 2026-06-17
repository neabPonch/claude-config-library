---
name: jackspace__ClaudeSkillz__skill-backup
source: https://github.com/jackspace/ClaudeSkillz/blob/fafc4690cff2a2420be1d0bd80a6d18c5091904a/skills/scientific-pkg-gtars/SKILL.md.backup
repo: jackspace/ClaudeSkillz
kind: skill
stars: 15
last_pushed: 2025-11-20T23:48:26Z
license: mit
score: 9
domains: [bioinformatics, cli-tools, data-science]
tags: [genomics, rust, python, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# jackspace/ClaudeSkillz — skill

**Why it's worth keeping:** Excellent use of 'When to use' sections to provide semantic intent and high-quality code examples that bridge individual functions into complete workflows.

**Summary:** Provides deep technical context for the gtars genomic analysis library, covering installation, API usage, and specific workflows.

**Source credibility:** High quality; based on a specialized open-source bioinformatics tool.

**Recency:** Current; includes modern packaging standards like uv.

**Source:** [jackspace/ClaudeSkillz/skills/scientific-pkg-gtars/SKILL.md.backup](https://github.com/jackspace/ClaudeSkillz/blob/fafc4690cff2a2420be1d0bd80a6d18c5091904a/skills/scientific-pkg-gtars/SKILL.md.backup) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gtars
description: High-performance toolkit for genomic interval analysis in Rust with Python bindings. Use when working with genomic regions, BED files, coverage tracks, overlap detection, tokenization for ML models, or fragment analysis in computational genomics and machine learning applications.
---

# Gtars: Genomic Tools and Algorithms in Rust

## Overview

Gtars is a high-performance Rust toolkit for manipulating, analyzing, and processing genomic interval data. It provides specialized tools for overlap detection, coverage analysis, tokenization for machine learning, and reference sequence management.

Use this skill when working with:
- Genomic interval files (BED format)
- Overlap detection between genomic regions
- Coverage track generation (WIG, BigWig)
- Genomic ML preprocessing and tokenization
- Fragment analysis in single-cell genomics
- Reference sequence retrieval and validation

## Installation

### Python Installation

Install gtars Python bindings:

```bash
uv pip install gtars
```

### CLI Installation

Install command-line tools (requires Rust/Cargo):

```bash
# Install with all features
cargo install gtars-cli --features "uniwig overlaprs igd bbcache
```

</details>
