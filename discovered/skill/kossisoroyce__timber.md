---
name: kossisoroyce__timber
source: https://github.com/kossisoroyce/timber/blob/151c6a68fe24c6dbbdcdc9c3c9c2330b4b11ce41/skill.md
repo: kossisoroyce/timber
kind: skill
stars: 684
last_pushed: 2026-04-16T16:38:25Z
license: other
score: 9
domains: [ml-ops, cli-tools, backend-api]
tags: [machine-learning, c99, deployment, performance]
curated: 2026-06-14
curated_by: config-scout
---

# kossisoroyce/timber — skill

**Why it's worth keeping:** The file provides perfect agent-facing documentation: explicit CLI command patterns, full HTTP request/response JSON schemas, and clear Python SDK usage examples which allow an agent to integrate the tool without ambiguity.

**Summary:** A highly structured skill reference for a tool that compiles classical ML models into high-performance C99 and serves them via an Ollama-compatible API.

**Source credibility:** High; well-starred repository with recent maintenance history.

**Recency:** Highly current, reflecting modern deployment workflows and Ollama compatibility.

**Source:** [kossisoroyce/timber/skill.md](https://github.com/kossisoroyce/timber/blob/151c6a68fe24c6dbbdcdc9c3c9c2330b4b11ce41/skill.md) · 684★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Timber — Coding Agent Skill Reference

> **For AI coding agents.** This file teaches you everything needed to use,
> integrate, and extend Timber without reading any other file.
> Version: 0.2.0

---

## What Timber does

Timber compiles a trained tree-based ML model (XGBoost, LightGBM, scikit-learn,
CatBoost, ONNX) into a self-contained C99 shared library and serves it over an
Ollama-compatible HTTP API. The compiled artifact has zero runtime dependencies
and runs at ~2 µs per sample.

**When to reach for Timber:**
- You need sub-millisecond tree model inference without Python overhead
- You want to serve a classical ML model the same way Ollama serves LLMs
- You need a portable C artifact for embedded, edge, or regulated environments
- You want a drop-in Ollama-compatible REST endpoint for a tree model

---

## Installation

```bash
pip install timber-compiler          # core (XGBoost, LightGBM, sklearn, ONNX, CatBoost)
pip install "timber-compiler[serve]" # + uvicorn for production HTTP
pip install "timber-compiler[full]"  # + all optional deps
```

**System requirement:** `gcc` or `clang` must be on `PATH`.

```bash
# verify
gcc --version || clang --version
python -c "import
```

</details>
