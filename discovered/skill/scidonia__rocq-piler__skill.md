---
name: scidonia__rocq-piler__skill
source: https://github.com/scidonia/rocq-piler/blob/6f68620a36f6a1a78e0ad0132025ecdbb3b3a260/src/skill.md
repo: scidonia/rocq-piler
kind: skill
stars: 8
last_pushed: 2026-06-10T05:21:43Z
license: apache-2.0
score: 9
domains: [formal-verification, software-engineering, logic]
tags: [coq, rocq, mcp, formal-methods, proof-assistant]
curated: 2026-06-16
curated_by: config-scout
---

# scidonia/rocq-piler — skill

**Why it's worth keeping:** Provides critical low-level logic like the 'Bullet rotation' system and a robust workflow for speculative lemma creation using `try_step` to avoid broken proof states.

**Summary:** A specialized skill file for performing formal verification in Coq/Rocq via MCP tools. It outlines specific workflows for theorem proving, lemma management, and bullet-based proof navigation.

**Source credibility:** Highly credible; leverages a specialized MCP server (`coq-lsp`) with active maintenance.

**Recency:** Very current, utilizing the updated 'Rocq' nomenclature and modern agentic tool patterns.

**Source:** [scidonia/rocq-piler/src/skill.md](https://github.com/scidonia/rocq-piler/blob/6f68620a36f6a1a78e0ad0132025ecdbb3b3a260/src/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Coq Proof Skill via MCP coq-lsp Tools

This document provides guidance for completing Coq/Rocq proofs using the `coq-lsp` MCP tools.

## Tool Reference

### Proof Navigation

| Tool | Purpose |
|------|---------|
| `focus_proof` | Get the current proof tree: goals, bullet depth, proof script up to cursor. Sets file cursor for subsequent `insert_tactic`. Accepts proof name or explicit position. |
| `open_goals` | Get current open goals for a named proof (Prev mode by default). |
| `proof_state` | Get richer proof context including proof name and statement. |
| `check_file` | Force full document checking and return completion status. |
| `check_file_range` | Check a specific line range and return diagnostics. |

### Tactic Insertion

| Tool | Purpose |
|------|---------|
| `insert_tactic` | Insert a tactic into a proof and return updated goals. **Auto-prepends bullet prefix** (-, +, *) when proof state requires it. Use `replace: true` to retry a failed tactic (undoes last insertion first). |
| `try_step` | Single-call speculative tactic execution: get state, run tactic, return updated goals. Does NOT modify the file. Use to test a tactic before committing. |
| `undo_step` | Restore
```

</details>
