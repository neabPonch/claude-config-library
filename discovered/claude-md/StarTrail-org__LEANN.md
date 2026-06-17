---
name: StarTrail-org__LEANN
source: https://github.com/StarTrail-org/LEANN/blob/cfb1382eccde2de8cd671a10ae0f251e35cf498b/CLAUDE.md
repo: StarTrail-org/LEANN
kind: claude-md
stars: 11924
last_pushed: 2026-06-15T04:00:36Z
license: mit
score: 9
domains: [ml-systems, cli-tools, backend-engine, rag]
tags: [vector-database, architecture-heavy, python-system]
curated: 2026-06-15
curated_by: config-scout
---

# StarTrail-org/LEANN — claude-md

**Why it's worth keeping:** The 'Self-Contained Principle' and technical pattern explanations (like the incremental update logic) are highly transferable techniques to prevent LLM context drift. The OS-specific dependency management is exceptionally thorough for agentic setup.

**Summary:** Provides deep architectural context alongside detailed multi-OS build instructions for complex C++ dependencies. Includes unique behavioral guidelines that enforce high-quality documentation through a 'Self-Contained Principle'.

**Source credibility:** High; high star count (11k+) and very recent activity indicate a major, well-maintained repository.

**Recency:** Very current; utilizes modern tooling like `uv`, `ruff`, and `claude.ai/code` specific instructions.

**Source:** [StarTrail-org/LEANN/CLAUDE.md](https://github.com/StarTrail-org/LEANN/blob/cfb1382eccde2de8cd671a10ae0f251e35cf498b/CLAUDE.md) · 11924★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LEANN is a lightweight vector database and RAG (Retrieval-Augmented Generation) system that achieves 97% storage reduction compared to traditional vector databases through graph-based selective recomputation. It enables semantic search across various data sources (emails, browser history, chat history, code, documents) on a single laptop without cloud dependencies.

## Build & Development Commands

### Quick install (pip)

```bash
pip install leann
```

### Development setup (from source)

```bash
# Install uv first (required package manager)
curl -LsSf https://astral.sh/uv/install.sh | sh

git submodule update --init --recursive

# macOS
brew install libomp boost protobuf zeromq pkgconf
uv sync

# Ubuntu/Debian
sudo apt-get install libomp-dev libboost-all-dev protobuf-compiler \
    libabsl-dev libmkl-full-dev libaio-dev libzmq3-dev
uv sync

# Windows (requires VS 2022 Build Tools with C++ workload, vcpkg, chocolatey)
choco install cmake swig pkgconfiglite nuget.commandline -y
vcpkg install zeromq:x64-windows openblas:x64-windows lapack:x64-wind
```

</details>
