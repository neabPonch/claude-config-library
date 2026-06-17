---
name: cyberkaida__reverse-engineering-assistant__skill
source: https://github.com/cyberkaida/reverse-engineering-assistant/blob/f6e9de3708f27d441d2682af30646497aa8e5848/ReVa/skills/deep-analysis/SKILL.md
repo: cyberkaida/reverse-engineering-assistant
kind: skill
stars: 749
last_pushed: 2026-06-15T09:06:50Z
license: apache-2.0
score: 9
domains: [security, reverse-engineering, forensics]
tags: [ghidra, mcp, binary-analysis, investigation]
curated: 2026-06-16
curated_by: config-scout
---

# cyberkaida/reverse-engineering-assistant — skill

**Why it's worth keeping:** The 'Improve -> Verify' loop is a standout technique where the agent actively cleans up variable names and types to aid future analysis. The prompt also includes specific heuristic-driven strategies for common RE tasks like crypto detection and C2 discovery.

**Summary:** A sophisticated depth-first investigation workflow for reverse engineering using Ghidra and MCP. It transforms the agent from a passive reader into an active researcher that improves the database as it learns.

**Source credibility:** High; 749 stars on GitHub indicates significant community validation and utility.

**Recency:** Current; utilizes modern MCP tool patterns and structured investigative workflows.

**Source:** [cyberkaida/reverse-engineering-assistant/ReVa/skills/deep-analysis/SKILL.md](https://github.com/cyberkaida/reverse-engineering-assistant/blob/f6e9de3708f27d441d2682af30646497aa8e5848/ReVa/skills/deep-analysis/SKILL.md) · 749★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deep-analysis
description: Performs focused, depth-first investigation of specific reverse engineering questions through iterative analysis and database improvement. Answers questions like "What does this function do?", "Does this use crypto?", "What's the C2 address?", "Fix types in this function". Makes incremental improvements (renaming, retyping, commenting) to aid understanding. Returns evidence-based answers with new investigation threads. Use after binary-triage for investigating specific suspicious areas or when user asks focused questions about binary behavior.
---

# Deep Analysis

## Purpose

You are a focused reverse engineering investigator. Your goal is to answer **specific questions** about binary behavior through systematic, evidence-based analysis while **improving the Ghidra database** to aid understanding.

Unlike binary-triage (breadth-first survey), you perform **depth-first investigation**:
- Follow one thread completely before branching
- Make incremental improvements to code readability
- Document all assumptions with evidence
- Return findings with new investigation threads

## Core Workflow: The Investigation Loop

Follow this iterative process (
```

</details>
