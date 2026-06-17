---
name: acidb__mobiscroll-demos
source: https://github.com/acidb/mobiscroll-demos/blob/01c24acef4e6d5daebe3ff3f061693e6111caf48/CLAUDE.md
repo: acidb/mobiscroll-demos
kind: claude-md
stars: 1
last_pushed: 2026-06-16T06:16:21Z
license: unknown
score: 8
domains: [web-frontend, monorepo]
tags: [multi-framework, automation, orchestration, meta-repository]
curated: 2026-06-17
curated_by: config-scout
---

# acidb/mobiscroll-demos — claude-md

**Why it's worth keeping:** Clearly documents high-level orchestration scripts (add/rename/sync) that maintain parity across subdirectories and warns about auto-generated files to prevent manual errors.

**Summary:** Defines a complex meta-repository structure used to manage UI component demos across seven different JavaScript frameworks.

**Source credibility:** Professional-grade documentation for a specialized UI library ecosystem.

**Recency:** Very current; references Vite v6, React v19, and Angular v21.

**Source:** [acidb/mobiscroll-demos/CLAUDE.md](https://github.com/acidb/mobiscroll-demos/blob/01c24acef4e6d5daebe3ff3f061693e6111caf48/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**mobiscroll-demos** is a meta-repository containing demo applications for the Mobiscroll UI components library across 7 different JavaScript frameworks:
- Angular (v21)
- JavaScript (vanilla)
- jQuery
- React (v19)
- React + TypeScript
- Vue 3
- Vue 3 + TypeScript

Each framework has its own subdirectory (`mobiscroll-demos-{framework}`) with a complete, independent demo application. The repository uses utility scripts to manage demos across all frameworks simultaneously.

## Repository Structure

### Root Level
- **package.json**: Contains root-level lint script and dependencies for utility scripts (fs-extra, mssql)
- **config.json**: Configuration pointing to external public demo repositories
- **Utility scripts** (Node.js):
  - `generate.js`: Queries Azure SQL database to generate demo lists and metadata
  - `add.js`: Scaffolds new demo files across all 7 frameworks using templates
  - `rename.js`: Renames/relocates demos while maintaining consistent structure across frameworks
  - `copy.js`: Syncs demos to separate public repositories
  - `re
```

</details>
