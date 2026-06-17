---
name: meirm__reverse-engineering-skill__skill-backup
source: https://github.com/meirm/reverse-engineering-skill/blob/be6b9fffa2db27b4ff43903448c60910b6c71f5b/.claude/skills/reverse-engineering-business-logic/SKILL.md.backup
repo: meirm/reverse-engineering-skill
kind: skill
stars: 18
last_pushed: 2026-03-17T12:54:59Z
license: unknown
score: 9
domains: [backend-architecture, reverse-engineering, documentation-as-code]
tags: [business-logic, domain-modeling, knowledge-base]
curated: 2026-06-16
curated_by: config-scout
---

# meirm/reverse-engineering-skill — skill

**Why it's worth keeping:** The 'Technical vs Business' translation framework and the strict mandate to save findings in a structured `business_logic/` directory with a master index create persistent, high-value documentation.

**Summary:** A specialized methodology for translating technical source code into domain-driven business documentation. It transforms an AI agent from a coder into a business analyst that documents 'what' a system does rather than just 'how'.

**Source credibility:** High-quality depth; 18 stars suggests niche popularity among developers interested in architecture.

**Recency:** Very current; uses modern frameworks like FastAPI and emphasizes Claude Code's tool-calling capabilities.

**Source:** [meirm/reverse-engineering-skill/.claude/skills/reverse-engineering-business-logic/SKILL.md.backup](https://github.com/meirm/reverse-engineering-skill/blob/be6b9fffa2db27b4ff43903448c60910b6c71f5b/.claude/skills/reverse-engineering-business-logic/SKILL.md.backup) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: reverse-engineering-business-logic
description: Reverse engineers business logic from source code by extracting operational business truth. Use when user asks to understand what the system actually does, analyze business rules, extract domain logic, infer workflows from code, explain state transitions, or identify decision logic. Works with Django views, FastAPI endpoints, models, Celery tasks, and multi-step workflows.
---

# Reverse Engineer Business Logic from Code

## Instructions

This skill extracts **business logic** from code, not technical implementation. The goal is to infer what the system actually does and express it in domain language, rules, workflows, edge cases, actors, and decisions.

### Core Principle

**Never confuse code structure with business structure.**

- Technical structure: `view -> serializer -> service -> provider -> model`
- Business structure: `validate request -> determine eligibility -> choose route -> execute lookup -> normalize result -> update record -> charge credits`

The distinction is the whole value.

### Prerequisites

None. Uses built-in tools (Read, Grep, Glob) to analyze source code.

### Workflow

#### Step 1: Identify the An
```

</details>
