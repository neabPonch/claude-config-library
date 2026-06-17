---
name: JetBrains__MPS__skill
source: https://github.com/JetBrains/MPS/blob/c8d3dc40717cf5ae91da732996d24415f72f57b8/.agents/skills/mps-node-editing/SKILL.md
repo: JetBrains/MPS
kind: skill
stars: 1648
last_pushed: 2026-06-16T21:03:34Z
license: apache-2.0
score: 9
domains: [meta-programming, dev-tools]
tags: [mps, node-manipulation, json-blueprints]
curated: 2026-06-17
curated_by: config-scout
---

# JetBrains/MPS — skill

**Why it's worth keeping:** It teaches a critical strategy of 'surgical edits' over 'full rewrites' to preserve persistent IDs and provides a specific workflow for handling large data payloads that exceed MCP transport limits.

**Summary:** A high-precision instruction set for performing surgical node mutations within the MPS meta-programming system using JSON blueprints.

**Source credibility:** Extremely high; developed by JetBrains, the industry leader in IDEs and meta-programming tools.

**Recency:** Current; according to metadata, it was updated within the last month.

**Source:** [JetBrains/MPS/.agents/skills/mps-node-editing/SKILL.md](https://github.com/JetBrains/MPS/blob/c8d3dc40717cf5ae91da732996d24415f72f57b8/.agents/skills/mps-node-editing/SKILL.md) · 1648★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mps-node-editing
description: Add, update, or delete MPS nodes using JSON blueprints — covers the unified blueprint format, staged construction for large subtrees, validation, and reference repair. Use whenever creating, editing, or restructuring nodes in any MPS model (structure, editor, behavior, generator, application code, etc.).
type: reference
---

# MPS Node Editing

The core workflow for mutating MPS nodes through MCP tools. JSON blueprints describe the node hierarchy you want; the tools resolve concepts, references, and used languages on insert.

## Critical Directives

- **Always use the fully qualified concept name** in the `concept` field — it is unambiguous and does not require a `conceptReference`.
- **Resolve before editing** — call `mps_mcp_get_current_editor_root_node` (for the user's focus) or `mps_mcp_search_root_node_by_name` (by name) to lock onto the target. Don't guess refs.
- **Prefer surgical edits** — `mps_mcp_update_node` (`ADD`/`CHILD` or `SET`/`CHILD`) preserves persistent IDs. `mps_mcp_update_root_node_from_json` rewrites the entire root and is wasteful when only one subtree changed.
- **Don't delete-and-reinsert** to make a small change — de
```

</details>
