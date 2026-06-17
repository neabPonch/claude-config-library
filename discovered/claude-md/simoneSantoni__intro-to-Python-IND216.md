---
name: simoneSantoni__intro-to-Python-IND216
source: https://github.com/simoneSantoni/intro-to-Python-IND216/blob/0b0c7b3a477bd59b5bd6eb29b4988938b3e15702/CLAUDE.md
repo: simoneSantoni/intro-to-Python-IND216
kind: claude-md
stars: 21
last_pushed: 2025-09-22T17:21:53Z
license: mit
score: 7
domains: [documentation, latex]
tags: [build-commands, latex, educational]
curated: 2026-06-16
curated_by: config-scout
---

# simoneSantoni/intro-to-Python-IND216 — claude-md

**Why it's worth keeping:** Explicitly documents necessary command-line arguments (-shell-escape) and the requirement for multiple compilation passes to resolve references.

**Summary:** Provides specific instructions for compiling LaTeX documentation that requires non-standard shell flags.

**Source credibility:** Low; small academic repository with 21 stars.

**Recency:** Current; standard LaTeX build workflows remain highly relevant for tool-use automation.

**Source:** [simoneSantoni/intro-to-Python-IND216/CLAUDE.md](https://github.com/simoneSantoni/intro-to-Python-IND216/blob/0b0c7b3a477bd59b5bd6eb29b4988938b3e15702/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an educational repository for "Introduction to Python - IND216/SMM692" course. The repository contains LaTeX-based course notes and supporting materials for teaching Python programming.

## Project Structure

- `notes/` - Main directory containing course materials
  - `notes.tex` - LaTeX source for course notes
  - `notes.pdf` - Compiled PDF output
  - `data/` - Sample data files used in examples
  - Various `.png` images - Screenshots and diagrams for the course
  - `.pgf` files - Plot graphics for the notes
  - `.npy`/`.npz` files - NumPy data files for examples

## Build Commands

### LaTeX Document Compilation
To compile the course notes PDF:
```bash
cd notes
pdflatex -shell-escape notes.tex
```
Note: The `-shell-escape` flag is required for the `minted` package used for code syntax highlighting.

For complete compilation with references and table of contents:
```bash
cd notes
pdflatex -shell-escape notes.tex
pdflatex -shell-escape notes.tex  # Run twice for references
```

## Key Dependencies

The LaTeX document uses:
- `minted` pack
```

</details>
