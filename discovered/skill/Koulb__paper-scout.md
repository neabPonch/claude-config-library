---
name: Koulb__paper-scout
source: https://github.com/Koulb/paper-scout/blob/c8b72b02dd8e8d46125296932f6dd3e459896eaa/SKILL.MD
repo: Koulb/paper-scout
kind: skill
stars: 0
last_pushed: 2026-06-05T15:05:53Z
license: unknown
score: 8
domains: [cli-tools, research-automation, agents-ai, data-collection]
tags: [academic, search-engine, sqlite, automation]
curated: 2026-06-14
curated_by: config-scout
---

# Koulb/paper-scout — skill

**Why it's worth keeping:** Uses 'single-driver' commands to wrap complex multi-step workflows (search/report/post) into high-level actions, reducing agent error. It also provides clear hierarchy of truth instructions for the agent.

**Summary:** A highly specific research automation CLI that manages academic paper discovery through arXiv and Google Scholar into a local SQLite database.

**Source credibility:** Low public visibility (0 stars), likely a specialized or private research tool.

**Recency:** Current; specifically designed with agentic automation and 'single-driver' patterns in mind.

**Source:** [Koulb/paper-scout/SKILL.MD](https://github.com/Koulb/paper-scout/blob/c8b72b02dd8e8d46125296932f6dd3e459896eaa/SKILL.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Paper Scout Skill

Search for academic papers and store them in a local SQLite database.

Current implementation can query **arXiv** and **Google Scholar**, but do **not** treat this file as the source of truth for search/ranking/filtering policy. Follow the latest instructions in the *paper-club* chat for paper-selection behavior.

## Installation

```bash
python3 -m venv .venv
./.venv/bin/pip install -r requirements.txt
```

Database-only commands work without those packages installed. Search commands need the relevant provider packages.

See `RECOMMENDATION_POLICY.md` for the current standing recommendation funnel, research tracks, and daily output expectations.

## Usage

Paper Scout runs as a Python CLI with three modes:

### 1. Database statistics (no arguments)

```bash
./.venv/bin/python search.py
```

Shows how many papers are in the database, broken down by source.

### 2. Search for papers

```bash
./.venv/bin/python search.py "electron-phonon coupling beyond DFT"
```

Runs the current configured search workflow, saves new papers to the database, and deduplicates by title hash. Use `-n` to control results per source:

```bash
./.venv/bin/python search.py "GW quasiparti
```

</details>
