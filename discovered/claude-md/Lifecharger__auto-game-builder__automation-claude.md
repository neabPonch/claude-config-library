---
name: Lifecharger__auto-game-builder__automation-claude
source: https://github.com/Lifecharger/auto-game-builder/blob/8040950d84e264f405ca23459f15235a1f9e6bbf/server/config/automation_claude.md
repo: Lifecharger/auto-game-builder
kind: claude-md
stars: 19
last_pushed: 2026-05-15T06:03:26Z
license: gpl-3.0
score: 9
domains: [game-development, agentic-workflows, mobile-dev]
tags: [micro-tasks, task-decomposition, godot, asset-generation, state-management]
curated: 2026-06-16
curated_by: config-scout
---

# Lifecharger/auto-game-builder — claude-md

**Why it's worth keeping:** The 'micro-task' decomposition logic and the formal workflow for splitting oversized tasks into a JSON tasklist are elite techniques for maintaining agent stability. It also includes proactive code safety patterns rather than reactive ones.

**Summary:** Establishes a rigid micro-tasking protocol to prevent agentic failure from large scopes and provides specific instructions for asset generation via external tools.

**Source credibility:** Written by an active developer of a niche game automation tool; shows high proficiency in both engine architecture and agent orchestration.

**Recency:** Very current, specifically addressing modern agent workflows like MCP tools and session-based task management.

**Source:** [Lifecharger/auto-game-builder/server/config/automation_claude.md](https://github.com/Lifecharger/auto-game-builder/blob/8040950d84e264f405ca23459f15235a1f9e6bbf/server/config/automation_claude.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Automation General Instructions

## Task Size Rules — MICRO TASKS ONLY
Every task you generate MUST be completable in a SINGLE session (max 30 minutes of AI work).

### What makes a good micro-task:
- ONE specific, clearly scoped change
- Touches at most 2-3 files
- Has a clear "done" condition that doesn't require visual testing
- Example: "Add health bar UI node to player scene" NOT "Implement full health system"
- Example: "Create inventory data model with item slots" NOT "Build inventory screen"
- Example: "Add jump animation state to player AnimationTree" NOT "Polish all player animations"
- Example: "Fix null check crash in score_manager.gd line 45" NOT "Fix all bugs on colony screen"

### What to NEVER generate:
- Vague tasks like "fill empty screen" or "implement X system end-to-end"
- Tasks that say "complete", "full", "entire", "all" — these are too big
- Tasks requiring multiple unrelated changes bundled together
- Tasks that need visual/manual testing to verify (the AI cannot see the screen)
- Tasks like "fix colony screen" — instead break into: "add colony list UI nodes", "connect colony data to UI labels", "add colony selection signal handler", etc.

### Task Genera
```

</details>
