---
name: rjs__shaping-skills__skill
source: https://github.com/rjs/shaping-skills/blob/d8b65d7733c71e9bf436f0c2e4da60e5214a96d9/breadboarding/skill.md
repo: rjs/shaping-skills
kind: skill
stars: 1360
last_pushed: 2026-04-10T10:12:59Z
license: unknown
score: 9
domains: [software-architecture, systems-design, ux-engineering]
tags: [mental-models, system-mapping, workflow-analysis, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# rjs/shaping-skills — skill

**Why it's worth keeping:** The 'Blocking Test' is a brilliant heuristic for defining bounded contexts, and the strict table output format prevents architectural vagueness. It is highly effective for reverse-engineering legacy systems or designing new ones through formal mental models.

**Summary:** This skill provides a rigorous methodology for mapping system workflows into structured 'affordance tables' and 'places'. It bridges the gap between high-level workflow descriptions and concrete technical implementation/analysis.

**Source credibility:** Highly credible; a popular repository with significant social proof (1360 stars) indicating a proven methodology.

**Recency:** Very current; provides high-value structural thinking required for modern agentic engineering workflows.

**Source:** [rjs/shaping-skills/breadboarding/skill.md](https://github.com/rjs/shaping-skills/blob/d8b65d7733c71e9bf436f0c2e4da60e5214a96d9/breadboarding/skill.md) · 1360★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: breadboarding
description: Transform a workflow description into affordance tables showing UI and Code affordances with their wiring. Use to map existing systems or design new ones from shaped parts.
---

# Breadboarding

Breadboarding transforms a workflow description into a complete map of affordances and their relationships. The output is always a set of tables showing numbered UI and Code affordances with their Wires Out and Returns To relationships. The tables are the truth. Mermaid diagrams are optional visualizations for humans.

---

## Use Cases

Breadboarding serves two functions:

### 1. Mapping an Existing System

You don't understand how an existing system works in its concrete details. You have a workflow you're trying to understand — explaining how something happens or why something doesn't happen.

**Input:**
- Code repo(s) to analyze
- Workflow description (always from the perspective of an operator trying to make an effect happen — through UI or as a caller)

**Output:**
- UI Affordances table
- Code Affordances table
- (Optional) Mermaid visualization

**Note:** If the workflow spans multiple applications (frontend + backend), create ONE breadboard that
```

</details>
