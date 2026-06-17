---
name: anik22889219__Aiagent
source: https://github.com/anik22889219/Aiagent/blob/abae822719b947a29e7cb1093997f53407af0ec8/claude.md
repo: anik22889219/Aiagent
kind: claude-md
stars: 0
last_pushed: 2026-03-05T06:13:38Z
license: unknown
score: 8
domains: [agents-ai, automation, systems-architecture]
tags: [agentic-workflow, separation-of-concerns, sop]
curated: 2026-06-14
curated_by: config-scout
---

# anik22889219/Aiagent — claude-md

**Why it's worth keeping:** Enforces the principle that business logic must be deterministic while LLM intelligence remains in orchestration, preventing 'probabilistic drift.' Includes a highly actionable self-healing loop for system improvement.

**Summary:** Implements a strict three-layer architecture separating high-level SOPs (Directives), AI reasoning (Orchestration), and deterministic Python tools (Execution).

**Source credibility:** Low social proof/stars, but demonstrates sophisticated architectural reasoning.

**Recency:** 

**Source:** [anik22889219/Aiagent/claude.md](https://github.com/anik22889219/Aiagent/blob/abae822719b947a29e7cb1093997f53407af0ec8/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Operating Instructions (Mirrored Across AGENTS.md, GEMINI.md)

This file defines how the AI system must operate.
It ensures reliability, determinism, and continuous self-improvement.

You operate inside a 3-layer architecture that separates reasoning from execution.

**LLMs are probabilistic. Business logic must be deterministic.**
This architecture prevents drift, inconsistency, and silent failures.

## 🔷 The 3-Layer Architecture

### Layer 1: Directives (What to Do)

**Location:** `/directives/`

These are Standard Operating Procedures written in Markdown.

Each directive must clearly define:

- Objective
- Inputs
- Expected Outputs
- Tools/Scripts to Use
- Edge Cases
- Error Handling
- Rate Limits (if API-based)

**Rules:**

- Directives are the source of truth.
- Do NOT override directives unless explicitly instructed.
- If something breaks, update the directive.
- Directives are living documents.

Think of directives as instructions you would give a mid-level employee.

### Layer 2: Orchestration (Decision Making) — This is You

You are the intelligent router and system manager.

**Your responsibilities:**

- Read the relevant directive.
- Check if a script already exi
```

</details>
