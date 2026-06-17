---
name: somnathrakshit__geograpy3
source: https://github.com/somnathrakshit/geograpy3/blob/c5a5bfe2fe0a2b6d451582987a689eaf8bb0919b/CLAUDE.md
repo: somnathrakshit/geograpy3
kind: claude-md
stars: 131
last_pushed: 2026-02-11T17:18:28Z
license: apache-2.0
score: 9
domains: [cli-tools, data-processing, nlp]
tags: [python, architecture-deep-dive, api-reference, testing-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# somnathrakshit/geograpy3 — claude-md

**Why it's worth keeping:** The file excels by providing architectural hierarchy (Extraction vs. Location stages) and specific testing setup patterns that prevent AI hallucinations about environment requirements.

**Summary:** Provides a comprehensive technical manual covering the two-stage processing pipeline, key class responsibilities, and critical command workflows.

**Source credibility:** Solid niche library with moderate social proof (131 stars) and clear documentation standards.

**Recency:** Highly relevant; follows modern developer-centric 'context-first' principles useful for Claude Code.

**Source:** [somnathrakshit/geograpy3/CLAUDE.md](https://github.com/somnathrakshit/geograpy3/blob/c5a5bfe2fe0a2b6d451582987a689eaf8bb0919b/CLAUDE.md) · 131★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

geograpy3 is a Python library that extracts place names (countries, regions, cities) from text or URLs and adds geographic context to them. It uses Natural Language Processing (NLTK) for entity recognition and Wikidata-derived databases for location disambiguation.

## Development Commands

### Installation
```bash
pip install .
geograpy-nltk  # Downloads required NLTK models
```

Or use the install script:
```bash
scripts/install
```

### Testing
```bash
# Run all tests
scripts/test

# Run with unittest directly
python3 -m unittest discover

# Run a single test file
python3 -m unittest tests.test_locator

# Run a specific test
python3 -m unittest tests.test_locator.TestLocator.test_issue_86
```

### Code Formatting
```bash
scripts/blackisort  # Runs isort and black on geograpy/ and tests/
```

### Documentation
```bash
scripts/doc  # Generates Sphinx documentation in docs/source
```

## Architecture

### Two-Stage Processing Pipeline

1. **Extraction Stage** (`extraction.py`): Uses NLTK to identify potential geographic entities in text
   - `Ext
```

</details>
