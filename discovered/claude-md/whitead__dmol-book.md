---
name: whitead__dmol-book
source: https://github.com/whitead/dmol-book/blob/34ff3fcfdc426b00f1e0f7851b8f9a6075c50b67/CLAUDE.md
repo: whitead/dmol-book
kind: claude-md
stars: 743
last_pushed: 2026-02-21T01:54:01Z
license: other
score: 9
domains: [data-science, machine-learning, education]
tags: [jupyter-book, migration-strategy, porting]
curated: 2026-06-15
curated_by: config-scout
---

# whitead/dmol-book — claude-md

**Why it's worth keeping:** The 'Porting Progress' section provides high-density state context that allows an agent to understand exactly what remains and the complexity involved. It also includes critical, non-obvious instructions for managing Jupyter Notebooks via TOC files.

**Summary:** A highly detailed guide for porting a Jupyter Book from TensorFlow to PyTorch. It outlines exact chapter-by-chapter progress and specific build/workflow procedures.

**Source credibility:** High; a well-starred (743) specialized educational repository.

**Recency:** Current; updated within the last 4 months.

**Source:** [whitead/dmol-book/CLAUDE.md](https://github.com/whitead/dmol-book/blob/34ff3fcfdc426b00f1e0f7851b8f9a6075c50b67/CLAUDE.md) · 743★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **Deep Learning for Molecules and Materials Book** (dmol.pub), a Jupyter Book-based educational resource covering deep learning applications in chemistry and materials science. The book uses Python with JAX, PyTorch, and scikit-learn, teaching concepts through interactive Jupyter notebooks.

## Project Status

We are porting version two from TensorFlow/Keras to PyTorch on the `v2` branch.

### Strategy

* Work down the `_toc.yml` file one by one by uncommenting chapters
* Build the book, observe errors in the most recently uncommented chapter
* Fix the errors, keeping the narrative close to the original text
* Commit as each cell is passing
* Ensure the text is consistent with the code modifications
* Update pseudocode snippets in markdown cells to use PyTorch syntax

### Porting Progress

**Completed (in `_toc.yml`, building):**
- `math/tensors-and-shapes` — no TF code, already fine
- `ml/introduction`, `ml/regression`, `ml/classification`, `ml/kernel` — no TF code, already fine
- `dl/introduction` — ported to PyTorch
- `dl/layers` —
```

</details>
