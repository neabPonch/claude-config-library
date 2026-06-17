---
name: derHaken__SuperAntigravity__skill
source: https://github.com/derHaken/SuperAntigravity/blob/2078b2c3d97f80976153c93ea4552495760a44d9/skills/confidence-check/SKILL.md
repo: derHaken/SuperAntigravity
kind: skill
stars: 435
last_pushed: 2026-02-27T17:16:25Z
license: mit
score: 9
domains: [agents-ai, software-engineering, developer-experience]
tags: [self-assessment, guardrails, context-verification, reliability]
curated: 2026-06-16
curated_by: config-scout
---

# derHaken/SuperAntigravity — skill

**Why it's worth keeping:** The 'Anti-Gaming Protocol' is brilliant; it requires the agent to provide concrete evidence (filenames/lines) for high scores, preventing vague overconfidence. It also provides a structured protocol for handling mid-implementation uncertainty.

**Summary:** A meta-cognitive self-assessment framework that forces an agent to verify understanding, context, and approach before implementation.

**Source credibility:** High; 435 stars indicates a widely recognized and useful toolset.

**Recency:** Very recent; perfectly applicable to current agentic workflows.

**Source:** [derHaken/SuperAntigravity/skills/confidence-check/SKILL.md](https://github.com/derHaken/SuperAntigravity/blob/2078b2c3d97f80976153c93ea4552495760a44d9/skills/confidence-check/SKILL.md) · 435★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: confidence-check
description: Use before implementing a feature or making significant changes to verify you have enough context and understanding to proceed — prevents wasted effort from proceeding with wrong assumptions
---

# Confidence Check

## Overview

A quick self-assessment before implementation. If confidence is below threshold,
gather more information first. Don't build on shaky understanding.

## When to Use

- Before starting implementation of a feature
- When requirements feel ambiguous
- After reading existing code that you're about to modify
- When you're unsure about a technical approach

## The Check

Score yourself 0-10 on each:

**Understanding (0-10)**
- Do I understand what this is supposed to do?
- Do I understand why it needs to exist?
- Do I understand who uses it and how?

**Context (0-10)**
- Do I know which files I need to touch?
- Do I understand the existing code patterns I'm building on?
- Do I know the data flow end-to-end?

**Approach (0-10)**
- Do I know which approach I'll take and why?
- Have I considered at least one alternative?
- Do I know how to test this?

## Anti-Gaming Protocol

This check fails its purpose if you score yourself 3
```

</details>
