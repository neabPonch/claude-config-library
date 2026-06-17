---
name: arach__arc__skill
source: https://github.com/arach/arc/blob/244175be25d8c510ef3c9c862ca5c3feada1cd21/docs/skill.md
repo: arach/arc
kind: skill
stars: 6
last_pushed: 2026-03-28T19:26:05Z
license: unknown
score: 8
domains: [web-frontend, diagramming-tools]
tags: [domain-knowledge, schema-driven, ui-components]
curated: 2026-06-16
curated_by: config-scout
---

# arach/arc — skill

**Why it's worth keeping:** Demonstrates how to use 'Triggers' and strict schema constraints (colors/sizes) to minimize AI hallucination; maps internal state logic to specific files for better agent navigation.

**Summary:** Provides high-density domain context, specific JSON schemas, and file system mappings for the Arc diagram engine.

**Source credibility:** Low star count, but the structured nature of the content indicates high-quality, intentional documentation for LLMs.

**Recency:** Current, utilizing modern tech stacks like React 19 and Vite 7.

**Source:** [arach/arc/docs/skill.md](https://github.com/arach/arc/blob/244175be25d8c510ef3c9c862ca5c3feada1cd21/docs/skill.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Arc Skills

> Pre-built skills for AI coding assistants working with Arc

## Available Skills

### arc-diagram

Create and modify Arc architecture diagrams.

**Trigger**: When user asks to create, edit, or work with architecture diagrams

**Capabilities**:
- Generate ArcDiagramData from natural language descriptions
- Add/remove/modify nodes and connectors
- Apply themes and styling
- Convert between JSON and TypeScript formats

**Context to provide**:
```
Arc diagram format: JSON with layout, nodes, nodeData, connectors, connectorStyles
Valid colors: violet, emerald, blue, amber, sky, zinc, rose, orange
Valid sizes: s, m, l
Valid anchors: left, right, top, bottom, topLeft, topRight, bottomLeft, bottomRight
Icons: Any Lucide icon name (Server, Database, Monitor, Cloud, etc.)
```

---

### arc-editor-dev

Develop and debug the Arc editor codebase.

**Trigger**: When working on Arc editor source code

**Context to provide**:
```
Arc Editor Structure:
- Entry: src/main.jsx → App.jsx
- Editor: src/components/editor/DiagramEditor.jsx
- State: EditorProvider.jsx + editorReducer.js (useReducer pattern)
- Canvas: DiagramCanvas.jsx (pointer events)
- Nodes: EditableNode.jsx (drag with poi
```

</details>
