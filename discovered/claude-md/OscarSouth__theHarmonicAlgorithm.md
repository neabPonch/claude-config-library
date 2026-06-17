---
name: OscarSouth__theHarmonicAlgorithm
source: https://github.com/OscarSouth/theHarmonicAlgorithm/blob/2fb1ee2670f74aed2a9f8b8f5c3214fbff74caa9/CLAUDE.md
repo: OscarSouth/theHarmonicAlgorithm
kind: claude-md
stars: 118
last_pushed: 2026-06-08T17:17:44Z
license: other
score: 9
domains: [haskell, music-theory, ai-agents, systems-architecture]
tags: [vertical-slices, mcp-memory, defensive-coding, test-driven]
curated: 2026-06-15
curated_by: config-scout
---

# OscarSouth/theHarmonicAlgorithm — claude-md

**Why it's worth keeping:** The use of a 'defensive' mindset (suspecting existing code) and the detailed orchestration of dual-system MCP memory (conversational vs. graph-based) are top-tier techniques.

**Summary:** This file provides an elite blueprint for agentic development by integrating strict verification protocols and explicit MCP memory management instructions.

**Source credibility:** High; the repo is actively maintained and demonstrates sophisticated integration of Haskell, Neo4j, and music theory.

**Recency:** Highly current; it directly leverages modern MCP tool usage patterns optimized for Claude Code.

**Source:** [OscarSouth/theHarmonicAlgorithm/CLAUDE.md](https://github.com/OscarSouth/theHarmonicAlgorithm/blob/2fb1ee2670f74aed2a9f8b8f5c3214fbff74caa9/CLAUDE.md) · 118★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# theHarmonicAlgorithm - Agent Guidelines

## Project Overview

A Haskell library for generating harmonic progressions trained on the Yale Classical Archives Corpus (YCACL). Uses Neo4j graph database for storing cadence transitions and integrates with TidalCycles for live music coding.

## Architecture

Four-layer system following Wiggins' Creative Systems Framework (R→E→T). For the full architecture, see [ARCHITECTURE.md](ARCHITECTURE.md).

Key directories:
- `src/Harmonic/Rules/Types/` - Music theory primitives (Pitch, Harmony, Progression)
- `src/Harmonic/Rules/Constraints/` - Filtering and validity rules (Filter, Overtone)
- `src/Harmonic/Rules/Import/` - Data ingestion pipeline (CSV, Transform, Graph)
- `src/Harmonic/Evaluation/` - Scoring and database queries (Dissonance, VoiceLeading, Query, Markov)
- `src/Harmonic/Traversal/` - Probabilistic selection
- `src/Harmonic/Framework/` - Builder (R→E→T orchestration)
- `src/Harmonic/Interface/Tidal/` - TidalCycles interface (Bridge, Arranger, Groove, Instruments, Utils)
- `test/` - HSpec + QuickCheck test suite
- `live/` - TidalCycles scripts and boot configuration

## Guiding Principles

### 1. Minimize Code and Complexity
The ov
```

</details>
