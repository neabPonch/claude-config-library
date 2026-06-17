---
name: pytorch__tutorials
source: https://github.com/pytorch/tutorials/blob/708b21c69bf42e10bc0226b8f4e580da839f24fe/CLAUDE.md
repo: pytorch/tutorials
kind: claude-md
stars: 9194
last_pushed: 2026-06-11T19:43:50Z
license: bsd-3-clause
score: 9
domains: [documentation, machine-learning, python]
tags: [sphinx, build-systems, workflow-guides]
curated: 2026-06-15
curated_by: config-scout
---

# pytorch/tutorials — claude-md

**Why it's worth keeping:** It includes hardware-aware build commands (GPU vs. no-GPU) and explicit tool prohibitions to prevent the AI from using incorrect linters.

**Summary:** Provides comprehensive build, linting, and contribution workflows for a documentation-heavy project using Sphinx.

**Source credibility:** Extremely high; PyTorch is a gold-standard open-source machine learning library.

**Recency:** Current; provides specific, actionable command patterns for modern documentation builds.

**Source:** [pytorch/tutorials/CLAUDE.md](https://github.com/pytorch/tutorials/blob/708b21c69bf42e10bc0226b8f4e580da839f24fe/CLAUDE.md) · 9194★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Structure

This is the PyTorch Tutorials website (`pytorch.org/tutorials`), built with Sphinx and Sphinx Gallery.

- `beginner_source/`, `intermediate_source/`, `advanced_source/`, `recipes_source/`, `unstable_source/` — tutorial source files (`.py` and `.rst`)
- `index.rst`, `recipes_index.rst` — card listings and toctrees for the website
- `conf.py` — Sphinx configuration (gallery dirs, extensions, theme)
- `_static/` — images, CSS, and thumbnails
- `requirements.txt` — all Python dependencies (Sphinx, tutorial packages)
- `.jenkins/` — CI build scripts, data download logic, post-processing
- `Makefile` — build entry points

Tutorials authored as `.py` files use Sphinx Gallery format: top-level docstrings become RST prose, code blocks become executable cells. These are executed during builds and converted to Jupyter notebooks and HTML. Tutorials authored as `.rst` are static and their code is not executed.

# Build

- `make html-noplot` — builds HTML without executing tutorial code. Fast, no GPU needed. Use this for quick validation of RST/Sphinx structure.
- `make docs` — full build that downloads data, executes all `.py` tutorials, and produces the final site. Require
```

</details>
