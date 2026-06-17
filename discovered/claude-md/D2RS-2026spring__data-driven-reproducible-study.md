---
name: D2RS-2026spring__data-driven-reproducible-study
source: https://github.com/D2RS-2026spring/data-driven-reproducible-study/blob/b47adc6ba658867571198752e936e15a25b0b08d/CLAUDE.md
repo: D2RS-2026spring/data-driven-reproducible-study
kind: claude-md
stars: 17
last_pushed: 2026-03-14T02:46:38Z
license: other
score: 9
domains: [data-science, academic-research, polyglot-environment]
tags: [quarto, r-lang, python, reproducible-research, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# D2RS-2026spring/data-driven-reproducible-study — claude-md

**Why it's worth keeping:** It excels at defining high-level cognitive workflows (e.g., the Slide Development Process) that guide an agent through research, drafting, and iterative refinement rather than just technical execution.

**Summary:** Provides comprehensive instructions for a complex polyglot environment involving R (renv), Python (Conda), and Quarto.

**Source credibility:** Academic course repository with active maintenance and specific toolchain integration.

**Recency:** Very current, referencing modern LLM tools and recent package management workflows.

**Source:** [D2RS-2026spring/data-driven-reproducible-study/CLAUDE.md](https://github.com/D2RS-2026spring/data-driven-reproducible-study/blob/b47adc6ba658867571198752e936e15a25b0b08d/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Quarto Book** for a university course on "Data Driven Reproducible Study" (数据驱动的可重复性研究). It teaches reproducible research practices using R, Python, Quarto, and modern AI/ML tools.

The book is bilingual (Chinese primary, English secondary) and covers:
- Environment setup (R, Python, Conda, Git)
- Data analysis (grouped data, transcriptomics, microbiome)
- AI/ML (neural networks from scratch, computer vision with PyTorch)
- LLM API integration (OpenAI, DeepSeek, Hugging Face)
- Collaboration (GitHub, R package development)

## Build Commands

### Render the Book

```bash
# Render entire book (HTML output)
quarto render

# Render to PDF (requires TinyTeX)
quarto render --to pdf

# Render specific file
quarto render grouped-data-analysis.qmd
```

### Clean Build Artifacts

```bash
make clean          # Remove _book/ directory
rm -rf _freeze      # Clear execution cache (if code chunks misbehave)
```

### Deploy

```bash
make deploy         # Run deployment script (_deploy.sh)
make book           # Render book via Makefile
```

### Updat
```

</details>
