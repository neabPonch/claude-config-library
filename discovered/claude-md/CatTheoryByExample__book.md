---
name: CatTheoryByExample__book
source: https://github.com/CatTheoryByExample/book/blob/2e6dd70f3a5d2b2992e21ed5931bf2d68d5ab45d/CLAUDE.md
repo: CatTheoryByExample/book
kind: claude-md
stars: 59
last_pushed: 2026-05-24T06:45:28Z
license: other
score: 9
domains: [latex, mathematics, publishing]
tags: [build-system, custom-macros, technical-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# CatTheoryByExample/book — claude-md

**Why it's worth keeping:** Explicitly defines custom mathematical macros and theorem environments to ensure consistency, and explains the necessity of specific build flags like -shell-escape and multiple PDF passes.

**Summary:** Detailed technical guide for building a complex LaTeX book with specific macro requirements and build-step explanations.

**Source credibility:** High; based on a well-structured academic book project with recent activity.

**Recency:** Very current, updated within the last month.

**Source:** [CatTheoryByExample/book/CLAUDE.md](https://github.com/CatTheoryByExample/book/blob/2e6dd70f3a5d2b2992e21ed5931bf2d68d5ab45d/CLAUDE.md) · 59★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a LaTeX book project titled "Category Theory by Example" by Ivan Murashko, Alexey Radkov, and Marat Minshin. The book covers category theory concepts with practical examples, including topics on Haskell and quantum mechanics.

## Build Commands

### Building the PDF
```bash
make
```

This command runs the complete LaTeX build pipeline:
- Compiles with `pdflatex` using `-shell-escape` flag (required for minted package)
- Processes bibliography with `bibtex`
- Generates nomenclature index with `makeindex`
- Runs `pdflatex` three times to resolve all cross-references

### Cleaning Build Artifacts
```bash
make clean
```

Removes all auxiliary files including:
- LaTeX auxiliary files (`.aux`, `.toc`, `.out`, `.idx`, `.nlo`, `.nls`)
- Bibliography files (`.bbl`, `.blg`)
- Log files (`.log`, `.ind`, `.ilg`)
- Minted cache directories (`_minted-*`)
- Backup files (`*~`)

## Project Structure

### Main Files
- `cattheory.tex` - Main LaTeX document that includes all chapters and defines custom macros, theorem environments, and document structure
-
```

</details>
