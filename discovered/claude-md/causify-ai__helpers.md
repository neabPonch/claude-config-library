---
name: causify-ai__helpers
source: https://github.com/causify-ai/helpers/blob/114581db5edefd622ccd6ae02a9c696584ee56ef/CLAUDE.md
repo: causify-ai/helpers
kind: claude-md
stars: 142
last_pushed: 2026-06-15T00:23:11Z
license: apache-2.0
score: 9
domains: [cli-tools, infrastructure, python]
tags: [modular-architecture, test-classification, task-automation]
curated: 2026-06-15
curated_by: config-scout
---

# causify-ai/helpers — claude-md

**Why it's worth keeping:** The explicit mapping of 'h<name>' module conventions and the classification of tests by execution time/infrastructure requirements allows Claude to choose the most efficient workflow immediately.

**Summary:** A comprehensive structural map of a large Python utility library that categorizes modules by function and defines a sophisticated task/test hierarchy.

**Source credibility:** High; part of an active, well-structured development system with 142 stars.

**Recency:** Current; tailored for modern tooling like Ruff and specifically addresses Claude Code workflows.

**Source:** [causify-ai/helpers/CLAUDE.md](https://github.com/causify-ai/helpers/blob/114581db5edefd622ccd6ae02a9c696584ee56ef/CLAUDE.md) · 142★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

# Repository Architecture

## Core Structure

This is the `helpers` repository, a foundational Python library providing
utilities, development tools, and infrastructure components for a larger
ecosystem. The codebase follows a modular architecture with these key
components:

- **`helpers/`**: Core utility modules (100+ modules) following `h<name>` naming
  convention organized into categories:
  - **Core Infrastructure**: `hdbg`, `hio`, `hsystem`, `hserver`, `henv` -
    debugging, I/O, system operations
  - **Data Processing**: `hpandas`, `hdataframe`, `hnumpy`, `hparquet`, `hcsv` -
    data manipulation and analysis
  - **Testing Framework**: `hunit_test`, `hpytest`, `hcoverage`, `hplayback` -
    comprehensive testing utilities
  - **External Services**: `haws`, `hs3`, `hgit`, `hdocker`, `hchatgpt`,
    `hllm` - cloud and tool integrations
  - **Caching & Performance**: `hcache`, `hcache_simple`, `hjoblib`, `htimer` -
    performance optimization
  - **Command-line & Parsing**: `hparser`: argument parsing and CLI utilities
  - **Text & Markdown**: `hmarkdown*` fam
```

</details>
