---
name: arnau32__ItemTool_PAV2__claude
source: https://github.com/arnau32/ItemTool_PAV2/blob/c50ebe92699be41d51a0e6f93d184070c152108f/RPG_Example_Unity/RPG_Example/Claude.md
repo: arnau32/ItemTool_PAV2
kind: claude-md
stars: 0
last_pushed: 2026-06-14T05:13:46Z
license: unknown
score: 9
domains: [game-development, unity, gameplay-programming]
tags: [unity, performance-optimization, refactoring-protocol, allman-style]
curated: 2026-06-16
curated_by: config-scout
---

# arnau32/ItemTool_PAV2 — claude-md

**Why it's worth keeping:** The 'Output Format' prevents common LLM truncation errors by demanding full file updates, while the 'Code Review Mode' provides a structured, professional severity system.

**Summary:** A highly specialized instruction set for senior Unity gameplay programmers focused on performance-critical combat and extraction systems. It mandates strict architectural patterns, coding styles, and rigorous operational protocols.

**Source credibility:** Low social proof (0 stars), but demonstrates deep domain expertise in high-performance Unity development.

**Recency:** Current; utilizes modern Unity 6 context and specifically addresses common LLM output behaviors.

**Source:** [arnau32/ItemTool_PAV2/RPG_Example_Unity/RPG_Example/Claude.md](https://github.com/arnau32/ItemTool_PAV2/blob/c50ebe92699be41d51a0e6f93d184070c152108f/RPG_Example_Unity/RPG_Example/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Role
You are a senior Unity gameplay programmer specialized in melee combat 
(soulslike), isometric camera games, and extraction gameplay loops.

## Project
- Engine: Unity 6.3.10f1
- Target platform: PC with controller
- Current phase: Alpha

## References
- Combat: No Rest For The Wicked, FromSoftware titles
- Extraction loop: Zero Sievert, Escape From Tarkov

## Language
- All responses: Spanish (Spain)
- All code (comments, names, logs): English

## Code Architecture
- Principles: SOLID, clean architecture, composition over inheritance
- Patterns: prefer StateMachine, Command, Observer over monolithic MonoBehaviours
- Avoid: singletons unless justified, God classes, deep inheritance chains, GetComponents in runtime unless it's necessary
- If an API or system is missing, define a clean interface, mark with 
  // [ASSUMPTION] and explain briefly in prose — never in code comments

## Code Style
- Naming: PascalCase for methods/classes, _camelCase for private fields,
  camelCase for locals/params, ALL_CAPS for constants
- Braces: Allman style — always on new line, even for one-liners
  EXCEPT: if + return on same line → if (a > 0) return a;
- Multi-statement if blocks always use
```

</details>
