---
name: Hazarre__pennylane-to-qiskit
source: https://github.com/Hazarre/pennylane-to-qiskit/blob/b8a98c57369d28e171dc18e5b754fd6ed8ea90b1/CLAUDE.md
repo: Hazarre/pennylane-to-qiskit
kind: claude-md
stars: 0
last_pushed: 2026-02-07T22:46:41Z
license: unknown
score: 7
domains: [agents-ai, quantum-computing]
tags: [knowledge-graph, agentic-workflow, code-translation]
curated: 2026-06-15
curated_by: config-scout
---

# Hazarre/pennylane-to-qiskit — claude-md

**Why it's worth keeping:** It documents high-level domain constraints (PennyLane vs Qiskit paradigms) and the specific multi-step execution cycle essential for debugging logic errors.

**Summary:** Explains a specialized agentic workflow for converting quantum computing code via knowledge graphs and iterative validation.

**Source credibility:** Low social proof (0 stars), but the technical depth suggests a legitimate, highly structured research project.

**Recency:** Recent; updated within the last 4 months.

**Source:** [Hazarre/pennylane-to-qiskit/CLAUDE.md](https://github.com/Hazarre/pennylane-to-qiskit/blob/b8a98c57369d28e171dc18e5b754fd6ed8ea90b1/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a research project focused on converting quantum computing programs from PennyLane to Qiskit using LLM agents with knowledge graph-based context. The system uses a knowledge graph to store mappings between PennyLane and Qiskit interfaces, then leverages this context to guide LLM-based code conversion.

### Key Concepts

- **Knowledge Graph (KG)**: Contains nodes representing PennyLane and Qiskit API components, and edges representing conversion/mapping relationships between them
- **Graph-based RAG**: The agent retrieves relevant conversion mappings from the KG to provide context for LLM-based code translation
- **Iterative Conversion**: The agent attempts conversion up to 3 times, executing and validating the generated Qiskit code against the original PennyLane program

## Architecture

### Core Components

1. **Knowledge Graph** (`knowledge_graph/`)
   - `p2q_kg.json` / `p2q_kg_light.json`: Main knowledge graphs with PennyLane-to-Qiskit mappings
   - `qml_kg.json`: PennyLane documentation nodes
   - `qiskit_kg.json`: Qiskit documentatio
```

</details>
