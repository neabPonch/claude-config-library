---
name: robinhenry__zotqa
source: https://github.com/robinhenry/zotqa/blob/a9345815f88649e1a3ed65b2fc1bfaae83c8d3ce/CLAUDE.md
repo: robinhenry/zotqa
kind: claude-md
stars: 2
last_pushed: 2026-02-14T09:00:20Z
license: mit
score: 8
domains: [cli-tools, data-engineering, rag]
tags: [zotero, python, rag, local-first]
curated: 2026-06-14
curated_by: config-scout
---

# robinhenry/zotqa — claude-md

**Why it's worth keeping:** The inclusion of a detailed 'Directory Structure' example and specific paths to local SQLite databases provides essential context that an LLM cannot guess.

**Summary:** Provides clear mapping of Zotero data extraction requirements and the target file system architecture for RAG.

**Source credibility:** Low star count, but demonstrates high-density domain expertise regarding Zotero's internal file structure.

**Recency:** Current; aligns with modern Python tooling (Poetry/Ruff) and agentic RAG workflows.

**Source:** [robinhenry/zotqa/CLAUDE.md](https://github.com/robinhenry/zotqa/blob/a9345815f88649e1a3ed65b2fc1bfaae83c8d3ce/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working on this repository.

## Project Overview

**zotqa** is a Python tool for querying an LLM agent (e.g., Claude API) about notes taken while reading papers in Zotero. It enables RAG (Retrieval Augmented Generation) over your Zotero library.

## Core Requirements

### Data Extraction from Zotero

For each paper in the Zotero library, extract:

1. **Metadata**
   - Title
   - Year
   - Authors
   - Abstract
   - Tags

2. **Notes**
   - All notes attached to the paper (Zotero stores these as child items)

3. **PDF Files**
   - The actual PDF attachment(s) for each paper

### Directory Structure for RAG

Organize extracted data in a directory structure optimized for LLM RAG workflows:

```
data/
├── papers/
│   ├── <paper_id>/
│   │   ├── metadata.json      # title, year, authors, abstract, tags
│   │   ├── notes.md           # concatenated notes in markdown
│   │   └── paper.pdf          # symlink to original PDF (avoid duplication)
│   └── ...
└── index.json                 # master index of all papers
```

## Technical Context

### Zotero Data Access

Read directly from the local Zotero SQLite database (no cloud API):
```

</details>
