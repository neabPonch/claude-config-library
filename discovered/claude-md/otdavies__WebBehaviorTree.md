---
name: otdavies__WebBehaviorTree
source: https://github.com/otdavies/WebBehaviorTree/blob/37d14d5bdc2b5a6cb4010c6b7f9ebc4c544d8b2f/claude.md
repo: otdavies/WebBehaviorTree
kind: claude-md
stars: 0
last_pushed: 2025-11-10T00:03:46Z
license: unknown
score: 9
domains: [web-frontend, graphics-engine]
tags: [canvas, typescript, architecture-driven]
curated: 2026-06-14
curated_by: config-scout
---

# otdavies/WebBehaviorTree — claude-md

**Why it's worth keeping:** The file excels at defining 'Mental Models' (Architecture Layers) and providing highly actionable constraints like specific Git commit rules and the 'Operation Pattern' to prevent naive refactors.

**Summary:** Provides deep architectural layers, strict coding standards, and performance-critical design principles for a canvas-based visual editor.

**Source credibility:** Low visibility (0 stars), but the technical depth suggests a professional-grade codebase.

**Recency:** Highly current; 7 months old is well within the relevance window for modern AI coding agents.

**Source:** [otdavies/WebBehaviorTree/claude.md](https://github.com/otdavies/WebBehaviorTree/blob/37d14d5bdc2b5a6cb4010c6b7f9ebc4c544d8b2f/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Browser-Based Behavior Tree Editor

Visual behavior tree editor built with vanilla TypeScript, HTML5 Canvas, and Monaco editor.

## Architecture Layers

```
Presentation  → editor/     (Canvas, rendering, interaction)
Application   → ui/         (Monaco, panels, toolbar)
              → state/      (Editor state management)
              → actions/    (Operation pattern implementations)
Domain        → core/       (Behavior tree logic, execution)
              → nodes/      (Node type implementations)
Infrastructure→ utils/      (File I/O, serialization, helpers)
```

## Core Principles

1. **Domain Independence**: Behavior tree logic has zero rendering dependencies
2. **Operation Pattern**: All mutations go through Operation objects (undo/redo ready)
3. **Spatial Indexing**: PortCache uses grid-based O(1) hit detection for performance
4. **Viewport Culling**: Only render visible nodes (optimized for large trees)
5. **Constants Extraction**: Magic numbers live in RendererConstants.ts

## File Organization

```
src/
├── core/           Domain logic - BehaviorTree, TreeNode, Blackboard, NodeExecutor
├── nodes/          Composites (Sequence/Selector/Parallel), Decorators, Leaves
├──
```

</details>
