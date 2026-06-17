---
name: eunomia-bpf__GPTtrace
source: https://github.com/eunomia-bpf/GPTtrace/blob/a1f83c7bf87c1114e97f714efb751bd510ea5d82/CLAUDE.md
repo: eunomia-bpf/GPTtrace
kind: claude-md
stars: 272
last_pushed: 2026-03-07T03:47:07Z
license: mit
score: 8
domains: [cli-tools, ai-agents, systems-programming]
tags: [python, architecture-mapping, dev-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# eunomia-bpf/GPTtrace — claude-md

**Why it's worth keeping:** The 'Code Architecture' section maps files to specific high-level behaviors (like retry mechanisms and function calling), allowing the agent to navigate logic instead of just file structures.

**Summary:** Provides comprehensive development lifecycle commands and a detailed architectural map of component responsibilities.

**Source credibility:** The repository has moderate star count and recent activity, indicating a real-world tool.

**Recency:** Highly current; utilizes modern Python tooling (ruff, mypy) and LLM patterns.

**Source:** [eunomia-bpf/GPTtrace/CLAUDE.md](https://github.com/eunomia-bpf/GPTtrace/blob/a1f83c7bf87c1114e97f714efb751bd510ea5d82/CLAUDE.md) · 272★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Install Dependencies
```bash
pip install -r requirements.txt
# or for development install
pip install -e .
```

### Run the Application
```bash
# Direct execution
python3 -m gpttrace "Your eBPF program request"

# With OpenAI API key
python3 -m gpttrace -k YOUR_API_KEY "Count page faults by process"

# Use bcc tool for tracing
python3 -m gpttrace -c CMD_NAME "Your query"

# Verbose mode
python3 -m gpttrace -v "Your request"
```

### Linting and Code Quality
```bash
# Run pylint (currently commented out in CI)
pylint $(git ls-files '*.py')

# Run ruff for linting (configured in pyproject.toml)
ruff check .

# Run mypy for type checking
mypy gpttrace

# Run code formatting with black and isort
black gpttrace
isort gpttrace
```

### Building and Publishing
```bash
# Build the package
python -m build

# Install locally in development mode
pip install -e .
```

## Code Architecture

### Core Components

1. **gpttrace/GPTtrace.py**: Main entry point that handles CLI argument parsing and routes to either `cmd` or `execute` functions

2. **gpttra
```

</details>
