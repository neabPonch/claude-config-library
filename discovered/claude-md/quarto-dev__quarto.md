---
name: quarto-dev__quarto
source: https://github.com/quarto-dev/quarto/blob/657c04b10422d15c2251c7ef71b2823f9c037457/claude.md
repo: quarto-dev/quarto
kind: claude-md
stars: 603
last_pushed: 2026-06-15T16:45:05Z
license: agpl-3.0
score: 8
domains: [monorepo, cli-tools, devops]
tags: [monorepo, turborepo, testing, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# quarto-dev/quarto — claude-md

**Why it's worth keeping:** It includes highly specific, agent-centric debugging instructions (e.g., using VERBOSE=1) and explicit guidance on how to interpret test output without over-filtering.

**Summary:** Provides a comprehensive map of a monorepo structure including build commands for different sub-projects.

**Source credibility:** High; Quarto is a well-established, actively maintained scientific publishing project.

**Recency:** Current; contains specific optimizations for Claude Code behavior.

**Source:** [quarto-dev/quarto/claude.md](https://github.com/quarto-dev/quarto/blob/657c04b10422d15c2251c7ef71b2823f9c037457/claude.md) · 603★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Quarto Development Guide

## Project Overview

Quarto is an open-source scientific and technical publishing system built on [Pandoc](https://pandoc.org). This repository contains the source code for various parts of the Quarto ecosystem, with the main CLI implementation housed in a separate repository ([quarto-cli](https://github.com/quarto-dev/quarto-cli)).

### Main Components

- **VS Code Extension**: The primary VS Code extension for working with Quarto documents
- **Writer**: An experimental web-based editor for Quarto documents (not used in production yet)
- **LSP**: Language server for Quarto documents
- **Core Packages**: Shared libraries used across multiple components

## Development Workflow

Each component has specific development guidelines. Refer to the corresponding CONTRIBUTING.md files:

- VS Code extension: [apps/vscode/CONTRIBUTING.md](apps/vscode/CONTRIBUTING.md) - Contains detailed instructions for building, debugging, and releasing the extension

## Repository Structure

The repository is organized as a monorepo using Yarn workspaces and Turborepo for build orchestration:

- `apps/`: Contains standalone applications
  - `vscode/`: VS Code extension for Quart
```

</details>
