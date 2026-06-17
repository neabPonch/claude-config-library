---
name: alexjungaalto__masterthesis
source: https://github.com/alexjungaalto/masterthesis/blob/0f105367f6c41c2ac68d7cd42cb02f4bd390e21a/CLAUDE.md
repo: alexjungaalto/masterthesis
kind: claude-md
stars: 26
last_pushed: 2026-06-15T07:32:28Z
license: mit
score: 8
domains: [data-management, documentation, cli-tools]
tags: [workflow-automation, build-instructions, csv-driven]
curated: 2026-06-15
curated_by: config-scout
---

# alexjungaalto/masterthesis — claude-md

**Why it's worth keeping:** It provides specific CLI commands to regenerate files, preventing the agent from wasting time editing files that will be overwritten by a script.

**Summary:** This file establishes clear boundaries between hand-editable 'sources of truth' and auto-generated build artifacts.

**Source credibility:** High; authored by an Associate Professor at Aalto University with a frequently updated repository.

**Recency:** Current; its instruction-heavy focus on CLI-driven workflows is ideal for modern agentic tool use.

**Source:** [alexjungaalto/masterthesis/CLAUDE.md](https://github.com/alexjungaalto/masterthesis/blob/0f105367f6c41c2ac68d7cd42cb02f4bd390e21a/CLAUDE.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

This is a **public GitHub repository** providing guidance to master thesis students supervised by Alex Jung (Associate Professor for Machine Learning, Aalto University). The audience is current and prospective supervisees.

## Repository Structure

- `README.md` — Main guide: supervisor/student expectations, getting started, timeline, writing conventions, evaluation process
- `topics.csv` — **Source of truth** for available thesis topic proposals. Hand-edit this file.
- `compile_topics.py` — Python script to compile and filter the topic catalog
- `Topics.md` — **Auto-generated** from `topics.csv` via `compile_topics.py` (do not edit directly)
- `theses.csv` — **Source of truth** for all supervised master theses (Aalto + TU Wien). Hand-edit this file.
- `compile_theses.py` — Python script to compile, filter, and export the thesis list
- `theses.md` — **Auto-generated** from `theses.csv` via `compile_theses.py` (do not edit directly)
- `theses.tex` — **Auto-generated** from `theses.csv` via `compile_theses.py` (do not edit directly)
- `material/` — PDFs and templates (grade characterization, self-assessment form, peer-review forms, current thesis lis
```

</details>
