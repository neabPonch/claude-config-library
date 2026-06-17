---
name: Cal2-0__Axon__axon-claude
source: https://github.com/Cal2-0/Axon/blob/14bd153ccec117a51ee434d2a735d1ddbc1f4e4a/backend/AXON_CLAUDE.md
repo: Cal2-0/Axon
kind: claude-md
stars: 0
last_pushed: 2026-06-14T15:41:08Z
license: unknown
score: 9
domains: [backend-api, security, data-processing]
tags: [architecture-first, performance-optimization, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# Cal2-0/Axon — claude-md

**Why it's worth keeping:** It uses the 'Problem vs. Solution' pattern to dictate exact data structures (e.g., Python sets for O(1) lookups) and orchestration logic (asyncio.gather), preventing the AI from introducing performance bottlenecks.

**Summary:** This file serves as a high-level architectural blueprint that mandates specific performance optimizations and concurrency patterns. It transitions from project context to detailed algorithmic constraints and implementation strategies.

**Source credibility:** Low repo reputation (0 stars, unknown license), but the technical depth suggests a highly skilled author.

**Recency:** Very current; uses modern Python async patterns and architectural styles suitable for contemporary development.

**Source:** [Cal2-0/Axon/backend/AXON_CLAUDE.md](https://github.com/Cal2-0/Axon/blob/14bd153ccec117a51ee434d2a735d1ddbc1f4e4a/backend/AXON_CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AXON — CLAUDE.md
## Blockchain Security Intelligence Platform
### Complete Pipeline Architecture, Efficiency Strategy & Development Specification

---

## 0. HOW TO READ THIS FILE

This is the single source of truth for building AXON. Every architectural decision is
documented here with its reasoning. Before writing any code, read the relevant section.
Sections are ordered by build priority — Phase 1 first, then refinements.

---

## 1. PROJECT CONTEXT

AXON is a blockchain forensics platform. The core loop is:

```
User submits a wallet address or contract address
       ↓
System fetches ALL available data from blockchain APIs
       ↓
System runs analysis (rules + ML + AI + DB lookup) in PARALLEL
       ↓
Results render progressively — graph and raw data first, AI verdict when ready
       ↓
Investigator sees a unified risk report with full evidence
```

The target user is a security analyst or forensic investigator who needs:
- Full transaction history (not sampled — every transaction)
- Risk score with explainable reasons
- Visual money flow graph
- AI-generated plain-English analysis
- Status visibility into which APIs are live

---

## 2. DIRECTORY STRUCTURE

```
axon/
├──
```

</details>
