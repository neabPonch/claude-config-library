---
name: anam-org__metaxy__skill
source: https://github.com/anam-org/metaxy/blob/df56a145eb1bf36e16a9d2a646a0c590176e5e19/.claude/skills/sybil/SKILL.md
repo: anam-org/metaxy
kind: skill
stars: 106
last_pushed: 2026-06-13T18:28:16Z
license: apache-2.0
score: 8
domains: [python, testing-infrastructure, documentation]
tags: [pytest, sybil, docstring-testing]
curated: 2026-06-15
curated_by: config-scout
---

# anam-org/metaxy — skill

**Why it's worth keeping:** Demonstrates complex integration patterns including custom evaluators, namespace management (setup/teardown), and conditional skip directives.

**Summary:** Provides comprehensive configuration patterns for Sybil, enabling automated validation of code examples in docstrings and Markdown files via pytest.

**Source credibility:** Decent; comes from an active repository with over 100 stars.

**Recency:** Highly relevant to contemporary Python development and testing workflows.

**Source:** [anam-org/metaxy/.claude/skills/sybil/SKILL.md](https://github.com/anam-org/metaxy/blob/df56a145eb1bf36e16a9d2a646a0c590176e5e19/.claude/skills/sybil/SKILL.md) · 106★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sybil
description: Use Sybil for testing code examples in documentation and docstrings. Covers pytest integration, parsers, skip directives, and namespace management.
---

# Sybil Documentation Testing

Sybil validates code examples embedded in documentation and docstrings by parsing and executing them as part of normal test runs.

**Official Documentation**: https://sybil.readthedocs.io/en/latest/

## Installation

```bash
pip install sybil[pytest]
```

## Pytest Integration

Configure in `conftest.py`. See [pytest integration docs](https://sybil.readthedocs.io/en/latest/integration.html#pytest-integration).

```python
from sybil import Sybil
from sybil.parsers.markdown.codeblock import PythonCodeBlockParser
from sybil.parsers.markdown.skip import SkipParser

pytest_collect_file = Sybil(
    parsers=[
        SkipParser(),
        PythonCodeBlockParser(),
    ],
    patterns=["*.md", "**/*.py"],
).pytest()
```

### Sybil Parameters

See [API reference](https://sybil.readthedocs.io/en/latest/api.html#sybil.Sybil).

| Parameter        | Description                                                     |
| ---------------- | ---------------------------------------------------
```

</details>
