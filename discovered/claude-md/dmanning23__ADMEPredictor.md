---
name: dmanning23__ADMEPredictor
source: https://github.com/dmanning23/ADMEPredictor/blob/1a1736a188a66d53b8b8db4236b9d0654d50c639/claude.md
repo: dmanning23/ADMEPredictor
kind: claude-md
stars: 0
last_pushed: 2026-03-17T04:52:17Z
license: unknown
score: 9
domains: [ml-engineering, api-design, ai-agents]
tags: [specification-driven, mcp-server, machine-learning, fullstack]
curated: 2026-06-16
curated_by: config-scout
---

# dmanning23/ADMEPredictor — claude-md

**Why it's worth keeping:** It provides exact function signatures, API schemas, and class definitions which act as a strict implementation contract for an LLM. It also includes highly specific instructions for building an MCP server, bridging the gap between raw ML logic and agentic tool use.

**Summary:** A comprehensive architectural blueprint for an end-to-end ML platform, covering backend API, GNN model structures, and MCP tool integration.

**Source credibility:** Low social proof (0 stars) but demonstrates high technical sophistication in computational chemistry/ML engineering.

**Recency:** Extremely current, incorporating modern standards like Model Context Protocol (MCP) and `uvx`.

**Source:** [dmanning23/ADMEPredictor/claude.md](https://github.com/dmanning23/ADMEPredictor/blob/1a1736a188a66d53b8b8db4236b9d0654d50c639/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ADME Predictor - Technical Implementation Guide

## Project Overview

This is a **free, open-source** portfolio project demonstrating end-to-end ML engineering skills applied to computational chemistry. It predicts ADME (Absorption, Distribution, Metabolism, Excretion) properties of drug-like molecules and is made available in three forms:

1. **Web Tool**: A hosted web application for interactive use (no account required)
2. **Public REST API**: An open API for programmatic access by developers and researchers
3. **MCP Server**: A Model Context Protocol server so LLM assistants (Claude, Cursor, etc.) can call ADME predictions as a tool during drug discovery workflows

The goal is to demonstrate proficiency in ML model training, API design, modern frontend development, and LLM tool integration — not to compete commercially with existing ADME platforms.

## Technology Stack

### Backend
- **Python 3.10+**
- **FastAPI**: REST API framework
- **PyTorch**: Deep learning framework
- **PyTorch Geometric**: Graph neural networks for molecular graphs
- **RDKit**: Chemistry toolkit for molecule manipulation
- **scikit-learn**: Classical ML baselines
- **Pydantic**: Data validation
- **Uvi
```

</details>
