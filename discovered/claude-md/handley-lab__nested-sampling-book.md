---
name: handley-lab__nested-sampling-book
source: https://github.com/handley-lab/nested-sampling-book/blob/d82a3370aa3f7cf4cd95cb5886fdbdae6f7a88d5/CLAUDE.md
repo: handley-lab/nested-sampling-book
kind: claude-md
stars: 3
last_pushed: 2026-06-10T14:14:30Z
license: mit
score: 8
domains: [scientific-computing, data-science]
tags: [jax, jupyter-book, algorithmic-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# handley-lab/nested-sampling-book — claude-md

**Why it's worth keeping:** The 'Key Patterns' section provides high-fidelity implementation templates that prevent hallucinations; the explicit git-tag dependency instruction ensures environment consistency.

**Summary:** Provides specific installation instructions for custom forks and detailed code patterns for core algorithmic workflows.

**Source credibility:** High-quality research repository with recent maintenance activity.

**Recency:** Current and highly relevant to modern JAX/scientific computing workflows.

**Source:** [handley-lab/nested-sampling-book/CLAUDE.md](https://github.com/handley-lab/nested-sampling-book/blob/d82a3370aa3f7cf4cd95cb5886fdbdae6f7a88d5/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jupyter Book repository containing educational notebooks demonstrating nested sampling algorithms from the BlackJAX library. The book focuses on physics-motivated use cases and provides pedagogical examples of nested sampling implementations.

The repository uses the nested sampling fork of BlackJAX from: https://github.com/handley-lab/blackjax (tag: `v0.1.0-beta`). This tag is for continuity while the merge into the main blackjax repository is in progress.

## Common Development Commands

### Building the Book
```bash
# Install dependencies
pip install -r requirements.txt

# Build the book locally
jupyter-book build .
# or shorthand
jb build .

# The built HTML will be in _build/html/
```

### Installation
```bash
# Install the nested sampling fork of BlackJAX
pip install git+https://github.com/handley-lab/blackjax.git@v0.1.0-beta

# Install visualization dependencies (for examples)
pip install anesthetic
```

### Contributing a New Example

1. Create a notebook in the appropriate directory:
   - `basic/` - Simple introductory examples
```

</details>
