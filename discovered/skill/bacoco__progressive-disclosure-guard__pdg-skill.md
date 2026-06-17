---
name: bacoco__progressive-disclosure-guard__pdg-skill
source: https://github.com/bacoco/progressive-disclosure-guard/blob/0df730a39dd2b9c928586b95a076cda9c80fcdb8/pdg.skill.md
repo: bacoco/progressive-disclosure-guard
kind: skill
stars: 1
last_pushed: 2026-06-07T08:33:37Z
license: mit
score: 9
domains: [agents-ai, software-engineering]
tags: [guardrails, reliability, verification, mission-control]
curated: 2026-06-14
curated_by: config-scout
---

# bacoco/progressive-disclosure-guard — skill

**Why it's worth keeping:** The 'Verification Protocol' (forcing the agent to name the specific command/route checked) and the 'Trigger Boundary' logic are elite techniques for ensuring reliability in tool-using agents.

**Summary:** A high-rigor guardrail system that forces AI agents to move from 'prose-based assumptions' to 'evidence-based verification'. It prevents mission drift and false claims of completion during complex architectural or code changes.

**Source credibility:** Low star count (1), but the sophisticated logical structure suggests an expert author deeply familiar with LLM failure modes.

**Recency:** Highly current; specifically designed for modern, tool-augmented coding agents like Claude Code.

**Source:** [bacoco/progressive-disclosure-guard/pdg.skill.md](https://github.com/bacoco/progressive-disclosure-guard/blob/0df730a39dd2b9c928586b95a076cda9c80fcdb8/pdg.skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: progressive-disclosure-guard
description: Use before finalizing specs, plans, implementation prompts, architecture reviews, UX critiques, handoff docs, code reviews, install/migration instructions, or after substantial code changes. Stay silent for typos, formatting-only edits, read-only lookups, one-command status checks, or low-risk changes with no handoff, behavior, or source-of-truth risk.
targets:
  - claude
  - codex
allowed-tools:
  - Read
  - Grep
  - Glob
  - Bash
context:
  - Read source-of-truth files before relying on memory.
  - Read relevant code before interpreting prose, inventories, or cited paths.
  - Inspect code, scripts, skills, agents, hooks, and configs before scoring reviews.
  - For risky skill calls, check skill usefulness twice and justify material unread files.
  - Keep checks bounded; do not recursively invoke PDG on PDG itself.
constitution:
  - progressive-disclosure-before-detail
  - evidence-before-claim
  - source-of-truth-before-memory
  - preserve-working-systems
  - separated-authority
  - real-verification-before-done
---

# PDG - Progressive Disclosure Guard

Use this skill before finalizing specs, plans, implementation prompts, arch
```

</details>
