---
name: engboris__stellogen
source: https://github.com/engboris/stellogen/blob/5b8dfa23387434f95af259f4fdc1c9e348a5b301/CLAUDE.md
repo: engboris/stellogen
kind: claude-md
stars: 137
last_pushed: 2026-03-30T22:12:45Z
license: gpl-3.0
score: 9
domains: [language-design, esoteric-languages, logic-programming]
tags: [unification, dsl, syntax-guide]
curated: 2026-06-15
curated_by: config-scout
---

# engboris/stellogen — claude-md

**Why it's worth keeping:** It bridges the gap between syntax and mental models via 'Core Philosophy' and provides actionable 'Common Patterns' to prevent the LLM from hallucinating standard Prolog behaviors.

**Summary:** Provides exhaustive domain knowledge for a custom esoteric language involving terms, rays, and star fusion.

**Source credibility:** High; clearly structured documentation for a specific research project.

**Recency:** Current; last updated 3 months ago.

**Source:** [engboris/stellogen/CLAUDE.md](https://github.com/engboris/stellogen/blob/5b8dfa23387434f95af259f4fdc1c9e348a5b301/CLAUDE.md) · 137★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Stellogen - Project Guide for Claude Code

## Overview

Stellogen is an experimental, **logic-agnostic** programming language based on **term unification**. It explores a radically different approach to programming where both computation and meaning are built from the same raw material, without primitive types or fixed logical rules imposed from above.

**Status:** Research project / proof of concept / esoteric language (not production-ready)

## Core Philosophy

Unlike traditional typed languages where types constrain and shape program design, Stellogen offers elementary interactive building blocks where computation and meaning coexist in the same language. The compiler/interpreter's role is reduced to checking that blocks connect - semantic power and responsibility belong entirely to the user.

## How Stellogen Works - Essential Mechanics

### 1. Terms - Everything is a Term
A **term** is either:
- **Variable**: Starts with uppercase (e.g., `X`, `Y`, `Result`)
  - Variables are local to each star
- **Function**: Lowercase/special symbol start with arguments in parentheses
  - Examples: `(f X)`, `(add X Y)`, `(s (s 0))`
  - Constants (0-arg functions) can omit parentheses: `a`,
```

</details>
