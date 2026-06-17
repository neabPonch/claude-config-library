---
name: microsoft__amplifier-bundle-systems-design__skill
source: https://github.com/microsoft/amplifier-bundle-systems-design/blob/1eff6a2bcebe7c42d5d8d4962e1937a3bb932b0c/skills/design-philosophy-object-oriented/SKILL.md
repo: microsoft/amplifier-bundle-systems-design
kind: skill
stars: 0
last_pushed: 2026-05-18T00:17:41Z
license: mit
score: 9
domains: [software-architecture, backend-engineering, design-patterns]
tags: [oop, solid, systems-design, heuristics]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/amplifier-bundle-systems-design — skill

**Why it's worth keeping:** The 'When it hurts' and 'Practical test' sections are elite; they prevent an agent from over-engineering by providing specific failure modes and heuristics.

**Summary:** Provides deep architectural reasoning for OO principles by focusing on 'managing the cost of change' rather than just definitions.

**Source credibility:** High quality content likely authored by experienced engineers, though the repository itself is niche (0 stars).

**Recency:** Timeless; these principles remain central to modern software engineering and AI code review.

**Source:** [microsoft/amplifier-bundle-systems-design/skills/design-philosophy-object-oriented/SKILL.md](https://github.com/microsoft/amplifier-bundle-systems-design/blob/1eff6a2bcebe7c42d5d8d4962e1937a3bb932b0c/skills/design-philosophy-object-oriented/SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: design-philosophy-object-oriented
description: "Object-oriented design principles as a lens for system architecture — SOLID, composition over inheritance, the actor model, design patterns (and when they're wrong), encapsulation, polymorphism, and responsibility-driven design. Use when evaluating code organization, module boundaries, or object/component relationships."
---

# Design Philosophy: Object-Oriented Design

OO principles as thinking tools for code organization, module boundaries, and component relationships.

---

## Core Premise

Object-oriented design is not about classes and inheritance. It is about **managing the cost of change** by localizing decisions behind stable interfaces. Every OO principle exists to answer one question: *when a requirement changes, how many places in the code must change with it?*

Good OO design means a single requirement change touches one or two files. Bad OO design means shotgun surgery across a class hierarchy that was supposed to make things "extensible."

The principles below are thinking tools, not commandments. Each one has a failure mode that is just as common as the problem it solves. Know both.

---

## 1. SOLID Principle
```

</details>
