---
name: codexceed__llm-chat
source: https://github.com/codexceed/llm-chat/blob/3b22d8c629dc890c4ecea78f37699b778f1853b3/CLAUDE.md
repo: codexceed/llm-chat
kind: claude-md
stars: 1
last_pushed: 2025-11-10T06:47:42Z
license: unknown
score: 8
domains: [agents-ai, rag-systems]
tags: [architecture, workflow, llm-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# codexceed/llm-chat — claude-md

**Why it's worth keeping:** Exemplary use of component mapping and design pattern explanations that provide high-level context beyond mere file locations.

**Summary:** A comprehensive guide covering development workflows and a deep architectural breakdown of an agentic RAG system.

**Source credibility:** Low star count (1), but documentation structure indicates highly organized research-oriented work.

**Recency:** Current; includes modern toolchain usage like uv and ruff.

**Source:** [codexceed/llm-chat/CLAUDE.md](https://github.com/codexceed/llm-chat/blob/3b22d8c629dc890c4ecea78f37699b778f1853b3/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

This is a learning project meant to help the developer understand the state-of-the-art in ML engineering concepts such as inference optimization, LLMs, agentic systems, distributed systems, etc.

## Development Commands

### Setup and Installation
```bash
make install-all              # Install all dependencies in development mode
make install-dev              # Install with development dependencies (uses uv)
make install-based            # Install base dependencies necessary to run the chatbot
make install-uv               # Install uv package manager (if needed)
```

### Code Quality and Linting
```bash
make lint-all                 # Run all linters and formatting (recommended)
make lint-fast                # Run fast running linters and formatters
make format                   # Format code with ruff
make lint                     # Check with ruff linter
make lint-fix                 # Auto-fix linting issues
make type-check               # Run mypy type checker
make security                 # Run bandit security scanner
make check                    # Quick vali
```

</details>
