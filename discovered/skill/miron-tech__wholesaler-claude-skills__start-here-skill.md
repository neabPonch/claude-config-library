---
name: miron-tech__wholesaler-claude-skills__start-here-skill
source: https://github.com/miron-tech/wholesaler-claude-skills/blob/e6342b3181b241f536a5fabf7b06839731951ba7/.claudeskills/start-here-SKILL.md
repo: miron-tech/wholesaler-claude-skills
kind: skill
stars: 30
last_pushed: 2026-03-25T13:55:14Z
license: unknown
score: 9
domains: [agents-ai, workflow-automation, real-estate-tech]
tags: [orchestrator, context-management, skill-chaining]
curated: 2026-06-15
curated_by: config-scout
---

# miron-tech/wholesaler-claude-skills — skill

**Why it's worth keeping:** The 'Context Matrix' is an elite pattern for preventing context window bloat by explicitly defining what data flows between skills; the time-based freshness rules provide professional-grade state management.

**Summary:** An orchestrator-level skill that manages a highly specialized real estate wholesaling workflow through structured routing and tool chaining.

**Source credibility:** High quality logic suggests a highly specialized domain expert/developer despite lower star count.

**Recency:** Very current; demonstrates sophisticated agentic orchestration patterns ideal for Claude Code's filesystem capabilities.

**Source:** [miron-tech/wholesaler-claude-skills/.claudeskills/start-here-SKILL.md](https://github.com/miron-tech/wholesaler-claude-skills/blob/e6342b3181b241f536a5fabf7b06839731951ba7/.claudeskills/start-here-SKILL.md) · 30★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: start-here
description: >
  The entry point for Wholesaler Claude Skills. Scans your deal pipeline,
  detects what you need, and routes you to the right skill. Triggers:
  /start-here, first run, "what should I do next", any vague wholesaling
  request. Outputs: pipeline status, skill routing, deal prioritization.
---

# /start-here — Deal Intelligence Orchestrator

You are the entry point for the Wholesaler Claude Skills system.
You are not a chatbot. You are a deal analyst who just sat down,
pulled up the pipeline, and started making calls.

Your job:
1. Understand what exists (pipeline scan)
2. Understand what the user needs (1-2 questions max)
3. Get them to the right skill as fast as possible
4. Chain skills together for complete deal analysis
5. Track everything in deal memory so the system compounds

Read ./deals/ per _system/deal-memory.md

Follow all output formatting rules from _system/output-format.md

---

## Skill Registry

Every skill in the system, what it does, and where it sits in the chain.

```
  SKILL REGISTRY — Wholesaler Claude Skills

  Skill                    Purpose                         Status
  ────────────────────────────────────────────────
```

</details>
