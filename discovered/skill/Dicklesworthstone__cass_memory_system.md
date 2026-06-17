---
name: Dicklesworthstone__cass_memory_system
source: https://github.com/Dicklesworthstone/cass_memory_system/blob/2e63e9ba81f155d48cfdc0f1d2c7d20a4996b3e9/SKILL.md
repo: Dicklesworthstone/cass_memory_system
kind: skill
stars: 380
last_pushed: 2026-06-06T04:01:25Z
license: other
score: 9
domains: [agents-ai, cli-tools, knowledge-management]
tags: [memory, cognitive-architecture, procedural-learning]
curated: 2026-06-14
curated_by: config-scout
---

# Dicklesworthstone/cass_memory_system — skill

**Why it's worth keeping:** The concept of 'Confidence Decay' (half-life) prevents rule obsolescence, while the automated inversion of failed rules into 'Anti-Patterns' provides high-value safety guardrails.

**Summary:** A cognitive architecture framework that transforms raw session logs into validated procedural rules using confidence decay and anti-pattern detection.

**Source credibility:** Strong; 380 stars indicates significant community validation and a well-maintained toolset.

**Recency:** Very current; specifically addresses cross-agent synchronization between tools like Claude Code and Cursor.

**Source:** [Dicklesworthstone/cass_memory_system/SKILL.md](https://github.com/Dicklesworthstone/cass_memory_system/blob/2e63e9ba81f155d48cfdc0f1d2c7d20a4996b3e9/SKILL.md) · 380★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cm
description: "CASS Memory System - procedural memory for AI coding agents. Three-layer cognitive architecture with confidence decay, anti-pattern learning, cross-agent knowledge transfer, trauma guard safety system. Bun/TypeScript CLI."
---

# CM - CASS Memory System

Procedural memory for AI coding agents. Transforms scattered sessions into persistent, cross-agent memory. Uses a three-layer cognitive architecture that mirrors human expertise development.

## Why This Exists

AI coding agents accumulate valuable knowledge but it's:
- **Trapped in sessions** - Context lost when session ends
- **Agent-specific** - Claude doesn't know what Cursor learned
- **Unstructured** - Raw logs aren't actionable guidance
- **Subject to collapse** - Naive summarization loses critical details

You've solved auth bugs three times this month across different agents. Each time you started from scratch.

CM solves this with cross-agent learning: a pattern discovered in Cursor is immediately available to Claude Code.

---

## Three-Layer Cognitive Architecture

```
┌─────────────────────────────────────────────────────────────────────┐
│                    EPISODIC MEMORY (cass)
```

</details>
