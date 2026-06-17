---
name: jiadong5__ZJU_PI_Thesis_Proposal
source: https://github.com/jiadong5/ZJU_PI_Thesis_Proposal/blob/68a02eba2b7e3eb9f28047edb62ed508c37461c8/CLAUDE.md
repo: jiadong5/ZJU_PI_Thesis_Proposal
kind: claude-md
stars: 11
last_pushed: 2026-03-05T02:08:52Z
license: unknown
score: 8
domains: [academic-writing, latex]
tags: [build-commands, formatting-rules]
curated: 2026-06-16
curated_by: config-scout
---

# jiadong5/ZJU_PI_Thesis_Proposal — claude-md

**Why it's worth keeping:** It provides exact shell commands for complex build chains and detailed stylistic rules (margins, numbering) to prevent AI formatting errors.

**Summary:** Defines a multi-pass XeLaTeX compilation sequence and strict formatting constraints for a university thesis.

**Source credibility:** Small academic repository with low star count but high specificity.

**Recency:** Current; last pushed 3 months ago.

**Source:** [jiadong5/ZJU_PI_Thesis_Proposal/CLAUDE.md](https://github.com/jiadong5/ZJU_PI_Thesis_Proposal/blob/68a02eba2b7e3eb9f28047edb62ed508c37461c8/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

Compile the LaTeX document using XeLaTeX (required for Chinese character support). All compilation artifacts are stored in `./claude_compile_temp/` directory.

**Full compilation with bibliography:**
```bash
xelatex -output-directory=./claude_compile_temp main.tex && \
biber --output-directory=./claude_compile_temp main && \
xelatex -output-directory=./claude_compile_temp main.tex && \
xelatex -output-directory=./claude_compile_temp main.tex && \
cp ./claude_compile_temp/main.pdf ./main.pdf
```

**Clean temporary files:**
```bash
rm -rf ./claude_compile_temp/*
```

## Project Structure

- **main.tex**: Main document source following Zhejiang University engineer school thesis proposal format
- **references.bib**: BibTeX bibliography database
- **imgs/**: Image assets directory
- **claude_compile_temp/**: Build artifacts directory (auto-created during compilation, gitignored)

## Document Configuration

- Document class: `article` (11pt) with `ctex` package for Chinese support
- Font setup: CMU Serif for Latin, Noto Serif CJK SC / Source Han Serif SC
```

</details>
