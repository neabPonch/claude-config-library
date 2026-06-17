---
name: ArchiveBox__abx-dl
source: https://github.com/ArchiveBox/abx-dl/blob/6409f78f4d515e2a8f1b20b9109e6898099a66c0/CLAUDE.md
repo: ArchiveBox/abx-dl
kind: claude-md
stars: 124
last_pushed: 2026-06-14T19:18:38Z
license: mit
score: 8
domains: [cli-tools, python]
tags: [cli, uv, testing-workflows, plugin-architecture]
curated: 2026-06-14
curated_by: config-scout
---

# ArchiveBox/abx-dl — claude-md

**Why it's worth keeping:** Includes 'manual testing' steps that allow an AI to verify changes in isolated environments, plus critical architectural context regarding how plugins and background hooks interact.

**Summary:** A highly specific guide for a Python CLI tool that provides detailed manual testing recipes and release protocols.

**Source credibility:** High; comes from a well-structured, actively maintained repository.

**Recency:** Very current; utilizes modern Python ecosystem tools like uv and ruff.

**Source:** [ArchiveBox/abx-dl/CLAUDE.md](https://github.com/ArchiveBox/abx-dl/blob/6409f78f4d515e2a8f1b20b9109e6898099a66c0/CLAUDE.md) · 124★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions for abx-dl

## Project Overview

abx-dl is a CLI tool for downloading URLs using ArchiveBox plugins. Plugins are symlinked from `/Users/squash/Code/ArchiveBox/archivebox/plugins` during development.

## Development Setup

```bash
# Install dependencies
uv sync --group dev

# Activate venv (or use uv run prefix)
source .venv/bin/activate
```

## Running Tests

### Manual testing in a temp directory
```bash
cd /tmp && rm -rf abx-dl-test && mkdir abx-dl-test && cd abx-dl-test
abx-dl dl --plugins=chrome,title 'https://example.com'

# Or test all plugins
abx-dl dl 'https://example.com'

# Check output
ls -la
cat title/title.txt
cat index.jsonl | jq -s '.'
```

### Running pytest
```bash
uv run pytest tests/
uv run pytest -xvs tests/  # verbose with output
```

## Linting

```bash
uv run ruff check abx_dl/
uv run ruff format abx_dl/
uv run mypy abx_dl/
```

## Rolling a New Release

1. **Bump version in pyproject.toml**
   ```bash
   # Edit version = "X.Y.Z" in pyproject.toml
   ```

2. **Commit, tag, and push**
   ```bash
   git add pyproject.toml
   git commit -m "Bump to vX.Y.Z"
   git push
   git tag -a vX.Y.Z -m "vX.Y.Z"
   git push origin vX.Y.Z
   ```

3
```

</details>
