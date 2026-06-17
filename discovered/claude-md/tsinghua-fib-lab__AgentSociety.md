---
name: tsinghua-fib-lab__AgentSociety
source: https://github.com/tsinghua-fib-lab/AgentSociety/blob/8cb830819da839028c1b2085e1475ebe26f13ee2/CLAUDE.md
repo: tsinghua-fib-lab/AgentSociety
kind: claude-md
stars: 1035
last_pushed: 2026-06-09T16:23:39Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, backend-api, research-framework]
tags: [architecture-diagrams, system-overview, uv-workspace]
curated: 2026-06-15
curated_by: config-scout
---

# tsinghua-fib-lab/AgentSociety — claude-md

**Why it's worth keeping:** The inclusion of a system architecture diagram and detailed 'Skill Architecture' explanations gives an agent the mental model needed to navigate complex dependencies without constant guessing.

**Summary:** Provides high-density architectural context using Mermaid diagrams and component breakdowns alongside specific development workflows.

**Source credibility:** High; well-maintained repository from a recognized research institution (Tsinghua) with high star count.

**Recency:** 

**Source:** [tsinghua-fib-lab/AgentSociety/CLAUDE.md](https://github.com/tsinghua-fib-lab/AgentSociety/blob/8cb830819da839028c1b2085e1475ebe26f13ee2/CLAUDE.md) · 1035★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository. For a shorter Cursor / agent entry point, see [AGENTS.md](./AGENTS.md).

## Project Overview

AgentSociety is a framework for building LLM-based agent simulations in urban environments and research workflows. The repository contains two main packages:

- **`packages/agentsociety`** (v1.x): City simulation framework with gRPC-based environment integration (legacy)
- **`packages/agentsociety2`** (v2.x): Modernized, LLM-native agent simulation platform with research skills (current focus)

## Workspace Structure

This is a uv workspace with Python packages in `packages/`:
- `packages/agentsociety2/` - Primary development package
- `packages/agentsociety/` - Legacy city simulation package
- `packages/agentsociety-community/` - Community contributions
- `packages/agentsociety-benchmark/` - Benchmarking utilities

The frontend is a separate React application in `frontend/`.
VSCode extension is in `extension/`.

## Development Commands

### Python Package (agentsociety2)

```bash
# Install dependencies (in workspace root)
uv sync

# Install with dev dependencies
cd packages/
```

</details>
