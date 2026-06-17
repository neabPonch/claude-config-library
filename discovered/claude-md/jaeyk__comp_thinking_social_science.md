---
name: jaeyk__comp_thinking_social_science
source: https://github.com/jaeyk/comp_thinking_social_science/blob/a19f78269a60f148a0cbc2786e8bb17fa241d5fb/CLAUDE.md
repo: jaeyk/comp_thinking_social_science
kind: claude-md
stars: 73
last_pushed: 2026-02-01T20:58:13Z
license: cc0-1.0
score: 7
domains: [data-science, documentation]
tags: [rstats, bookdown, static-site]
curated: 2026-06-16
curated_by: config-scout
---

# jaeyk/comp_thinking_social_science — claude-md

**Why it's worth keeping:** Excellent inclusion of multiple build commands (full vs. fast) and explicit documentation of environmental quirks like session handling and encoding requirements.

**Summary:** Defines specific build workflows, project structure, and environment configurations for an R bookdown repository.

**Source credibility:** Moderate; 73 stars indicates a respected educational resource.

**Recency:** 

**Source:** [jaeyk/comp_thinking_social_science/CLAUDE.md](https://github.com/jaeyk/comp_thinking_social_science/blob/a19f78269a60f148a0cbc2786e8bb17fa241d5fb/CLAUDE.md) · 73★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a bookdown project for "Computational Thinking for Social Scientists" - an educational textbook teaching computational methods to social scientists. The book covers R programming, data wrangling, functional programming, APIs/web scraping, machine learning, and SQL.

## Build Commands

```bash
# Build all formats (HTML, PDF, EPUB)
bash _build.sh

# Or directly via R
Rscript -e "bookdown::render_book('.', output_format = 'all')"

# Build HTML only (faster)
Rscript -e "bookdown::render_book('.', output_format = 'bookdown::gitbook')"
```

Output is generated in the `docs/` directory. Open `docs/index.html` to preview.

## Project Structure

- `index.Rmd` - Book front matter and introduction
- `01_motivation.Rmd` through `08_big_data.Rmd` - Chapter content
- `_common.R` - Shared R configuration run before each chapter
- `_bookdown.yml` - Bookdown configuration
- `_output.yml` - Output format settings
- `docs/` - Generated output (HTML, PDF, EPUB)

## Key Configuration

- Each chapter runs in a fresh R session (`new_session: true`)
- Uses xelat
```

</details>
