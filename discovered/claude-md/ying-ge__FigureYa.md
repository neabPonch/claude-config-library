---
name: ying-ge__FigureYa
source: https://github.com/ying-ge/FigureYa/blob/f627917b79f28558779fb2e3ea2014cede41b89e/CLAUDE.md
repo: ying-ge/FigureYa
kind: claude-md
stars: 383
last_pushed: 2026-01-21T04:19:51Z
license: other
score: 8
domains: [data-science, bioinformatics, reproducible-research]
tags: [RMarkdown, module-based, scientific-computing]
curated: 2026-06-15
curated_by: config-scout
---

# ying-ge/FigureYa — claude-md

**Why it's worth keeping:** The 'Module Structure Pattern' and 'Creating New Modules' sections provide perfect blueprints for an AI to generate new, consistent project components.

**Summary:** Defines a highly structured, module-based architecture for scientific R Markdown reports, including specific execution and creation workflows.

**Source credibility:** Well-maintained biomedical repository with significant community interest (383 stars).

**Recency:** Recent activity (5 months ago) makes it highly relevant for current development workflows.

**Source:** [ying-ge/FigureYa/CLAUDE.md](https://github.com/ying-ge/FigureYa/blob/f627917b79f28558779fb2e3ea2014cede41b89e/CLAUDE.md) · 383★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**FigureYa** is a comprehensive biomedical data visualization framework providing 300+ standardized R Markdown templates for creating scientific figures. It's designed for genomic, transcriptomic, proteomic, and clinical biomedical research, emphasizing reproducibility and scientific best practices.

## Common Development Commands

### Running Individual Modules
Each module (FigureYaXXX directory) can be executed independently:

```bash
# Navigate to a specific module
cd FigureYa101PCA

# Install dependencies (automatic within RMD, but can be run manually)
Rscript install_dependencies.R

# Execute the analysis and generate HTML report
R -e "rmarkdown::render('FigureYa101PCA.Rmd')"
```

### Build and Automation Commands
The repository uses GitHub Actions for automation:

- **Search index generation**: Automatically runs on main branch pushes
- **Gallery compression**: Handles large image files
- **Repository synchronization**: Maintains file consistency

For local development of the search interface:
```bash
# Requires Python and beautifulsoup4
pi
```

</details>
