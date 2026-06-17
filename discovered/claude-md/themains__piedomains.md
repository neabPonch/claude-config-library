---
name: themains__piedomains
source: https://github.com/themains/piedomains/blob/9d2164a9007c558d7a286129dbaba313e0e3cb75/CLAUDE.md
repo: themains/piedomains
kind: claude-md
stars: 16
last_pushed: 2025-12-20T03:48:10Z
license: mit
score: 9
domains: [machine-learning, python]
tags: [ml-ops, architecture-documentation, pipeline-context]
curated: 2026-06-15
curated_by: config-scout
---

# themains/piedomains — claude-md

**Why it's worth keeping:** The structured 'Architecture' and 'Machine Learning Pipeline' sections provide deep context on component dependencies and data transformations. It also includes critical operational details like memory management and security constraints that guide the AI toward safer coding practices.

**Summary:** This file provides a comprehensive blueprint of an ML pipeline, detailing command patterns, modular architecture, and data flow. It is highly effective at explaining how specific components interact within a complex processing workflow.

**Source credibility:** While a smaller project (16 stars), the highly structured documentation suggests a high-quality, professional codebase.

**Recency:** Current; pushed 6 months ago, making it relevant for modern Claude Code workflows.

**Source:** [themains/piedomains/CLAUDE.md](https://github.com/themains/piedomains/blob/9d2164a9007c558d7a286129dbaba313e0e3cb75/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Testing
- Run all tests: `pytest tests/ -v`
- Run tests without ML models: `pytest tests/ -v -m "not ml"`
- Run specific test: `pytest tests/test_001_pred_domain_text.py`
- Run with coverage: `pytest tests/ --cov=piedomains`

### Linting and Code Quality
- Run pylint: `pylint piedomains/` (uses configuration from `pylintrc`)
- Run flake8 (CI configuration): 
  - Syntax errors: `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`
  - General linting: `flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics`

### Installation and Development
- Install package: `pip install -e .` (from repository root)
- Install with dev dependencies: `pip install -e ".[dev]"`
- Console script: `classify_domains` (entry point defined in pyproject.toml)

### Package Management
- Build package: `python -m build`
- Upload to PyPI: `python -m twine upload dist/*`
- Validate README: `python -c "import docutils.core; docutils.core.publish_doctree(open('README.rst').read())"`

### Documentation
- Build docs: `cd docs && make html`
-
```

</details>
