---
name: vincentarelbundock__tinytable
source: https://github.com/vincentarelbundock/tinytable/blob/e21e6929d33fec0f34e2b4cb1018491078fd4e1d/CLAUDE.md
repo: vincentarelbundock/tinytable
kind: claude-md
stars: 333
last_pushed: 2026-06-07T01:19:00Z
license: gpl-3.0
score: 9
domains: [data-visualization, r-programming, package-development]
tags: [S4-classes, lazy-evaluation, unit-testing, R]
curated: 2026-06-15
curated_by: config-scout
---

# vincentarelbundock/tinytable — claude-md

**Why it's worth keeping:** It documents internal state dependencies (e.g., that S4 slots are only populated upon printing), which prevents an AI from making incorrect debugging assumptions about object attributes.

**Summary:** This file provides deep technical insights into the package's S4 class architecture and lazy evaluation patterns. It includes specific R-specific workflows for testing, documentation, and development.

**Source credibility:** High; it is a well-maintained R package with significant community interest.

**Recency:** 

**Source:** [vincentarelbundock/tinytable/CLAUDE.md](https://github.com/vincentarelbundock/tinytable/blob/e21e6929d33fec0f34e2b4cb1018491078fd4e1d/CLAUDE.md) · 333★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## User instructions

Whenever running code from this package, always run `pkgload::load_all()` first to ensure the latest version is loaded. Never use `library(tinytable)`.

To run all tests: `pkgload::load_all(); tinytest::run_test_dir()`

Many operations inside `tinytable` are "lazy", and the S4 slots will not be filled until a table is "built". To build a table in a given format, call `print(x, "html")` or `build_tt(x, "html")` where `x` is a `tinytable` object. This will trigger the lazy evaluation and fill the S4 slots with the necessary data.

`x@style` is only filled on print, so use `print(x, "html")` and `cat()` to debug.

### Development workflow
- Always use `pkgload::load_all()` before testing any code changes
- Test changes with specific test files: `tinytest::run_test_file("inst/tinytest/test-html.R")`
- Use `make check` to run R CMD check before committing changes

## Project Overview

`tinytable` is an R package for creating tables in HTML, LaTeX, Markdown, Word, PDF, PNG, and Typst formats. Zero-dependency design (only `methods` package). User inter
```

</details>
