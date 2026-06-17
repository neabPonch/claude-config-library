---
name: omagm__new_taxonomy
source: https://github.com/omagm/new_taxonomy/blob/ae059acbf8051accb65ab69e48f50916fa9d9c51/claude.md
repo: omagm/new_taxonomy
kind: claude-md
stars: 0
last_pushed: 2025-11-10T16:25:23Z
license: unknown
score: 7
domains: [data-modeling, mcp-server, workflow-automation]
tags: [schema-sync, dependency-management, side-effects]
curated: 2026-06-16
curated_by: config-scout
---

# omagm/new_taxonomy — claude-md

**Why it's worth keeping:** Uses an 'Important Note' to explicitly document the necessary side effects when changing core schemas, preventing broken dependencies across MCP tools and data files.

**Summary:** Defines a machine taxonomy system and enforces a rigorous synchronization protocol for schema changes.

**Source credibility:** Low; repository has 0 stars and no specific author reputation provided.

**Recency:** Current; focuses on a multi-step workflow essential for maintaining MCP server consistency.

**Source:** [omagm/new_taxonomy/claude.md](https://github.com/omagm/new_taxonomy/blob/ae059acbf8051accb65ab69e48f50916fa9d9c51/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
This repo is about a machines taxonomy management system spanning categories, specification groups, specifications and presets.

In taxonomy_description.md the new system to manage machine taxonomies is described.


```/app``` contains the MCP server to manage data. It can be connected to Claude Desktop or others to manage the tree via chat.

```/schemas``` contains the schema definitions for the data models used in the MCP server. 

```/data``` contains JSON data files with machine taxonomies and models.

```/interface``` a small web app to render a collapsible category tree as a HTML page.

**Important Note:** Whenever changing the schema definitions in ```/schemas```, the following has to be done right after it:
1) Schema Package has to be rebuilt so that the Typescript types are updated as well.
2) The MCP server has to adjust its tool functions to support the changes. It also has to be restarted to load the new schema definitions.
3) The JSON data files in ```/data``` have to be checked for compliance with the new schema definitions. If necessary, they have to be updated to conform to the new schema.
4) The web app in ```/interface``` may need to be updated to reflect any chan
```

</details>
