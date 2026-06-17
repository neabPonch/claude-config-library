---
name: Snagnar__Factompiler__claude-md
source: https://github.com/Snagnar/Factompiler/blob/957485d2f85b775fa2074071377dadd969e37a35/dsl_compiler/src/layout/CLAUDE.MD
repo: Snagnar/Factompiler
kind: claude-md
stars: 409
last_pushed: 2026-05-18T13:22:58Z
license: mit
score: 8
domains: [compilers, systems-programming]
tags: [architecture, data-flow, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# Snagnar/Factompiler — claude-md

**Why it's worth keeping:** The 'Information Flow' ASCII diagram and explicit mapping of files to specific roles provide essential context for an AI to understand dependency chains and data transformations before editing code.

**Summary:** Acts as a high-density architectural blueprint defining module responsibilities and execution pipelines.

**Source credibility:** Highly credible; the source is a specialized, complex compiler project with significant community traction (409 stars).

**Recency:** Very recent; last pushed 1 month ago, making it highly relevant for current agentic workflows.

**Source:** [Snagnar/Factompiler/dsl_compiler/src/layout/CLAUDE.MD](https://github.com/Snagnar/Factompiler/blob/957485d2f85b775fa2074071377dadd969e37a35/dsl_compiler/src/layout/CLAUDE.MD) · 409★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Layout Module

## Purpose
Converts IR operations into physical layouts - determines where to place combinators, how to wire them, and how to power them. This is the most complex stage of compilation.

## Files

### planner.py
**Main Layout Orchestrator**
- `LayoutPlanner`: Coordinates physical layout planning
  - Entry: `plan_layout(ir_ops)` → `LayoutPlan`
  - Delegates to specialized planners
  - Manages entity placement, wiring, and power

### layout_plan.py
**Layout Data Structure**
- `LayoutPlan`: Container for complete layout information
  - Entity placements (combinators, poles, lamps, etc.)
  - Wire connections (red/green wires)
  - Tile placements
  - Entity configurations

- `EntityPlacement`: Represents a placed entity
  - Position (x, y)
  - Entity type
  - Configuration (control behavior, filters, etc.)

### entity_placer.py
**Combinator Placement**
- `EntityPlacer`: Places combinators for IR operations
  - Arithmetic → Arithmetic combinator
  - Decider → Decider combinator
  - Constant → Constant combinator
  - Memory → Memory cell (combinator pair)
  - Determines positions using grid-based placement

### signal_analyzer.py
**Signal Flow Analysis**
- `SignalAnalyzer`
```

</details>
