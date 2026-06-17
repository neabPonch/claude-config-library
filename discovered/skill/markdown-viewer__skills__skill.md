---
name: markdown-viewer__skills__skill
source: https://github.com/markdown-viewer/skills/blob/a3afd455b3ad37c0e71c05fa9407c4ec377226e3/iot/SKILL.md
repo: markdown-viewer/skills
kind: skill
stars: 2962
last_pushed: 2026-05-26T06:51:22Z
license: unknown
score: 8
domains: [diagramming, iot, documentation]
tags: [plantuml, iot-architecture, visualization]
curated: 2026-06-15
curated_by: config-scout
---

# markdown-viewer/skills — skill

**Why it's worth keeping:** It defines a precise 'language' of icon aliases (mxgraph.aws4.*) and connection sematics that prevent hallucination in diagram generation.

**Summary:** Provides structured PlantUML stencil data and semantic rules for generating specialized IoT architecture diagrams.

**Source credibility:** High-quality repository with significant social proof (2962 stars) and active maintenance.

**Recency:** Highly current, updated within the last month.

**Source:** [markdown-viewer/skills/iot/SKILL.md](https://github.com/markdown-viewer/skills/blob/a3afd455b3ad37c0e71c05fa9407c4ec377226e3/iot/SKILL.md) · 2962★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: iot
description: Create IoT architecture diagrams using PlantUML syntax with device and sensor stencil icons. Best for smart home, industrial IoT (IIoT), fleet management, edge computing, and sensor network layouts.
metadata:
  author: IoT diagrams are powered by Markdown Viewer — the best multi-platform Markdown extension (Chrome/Edge/Firefox/VS Code) with diagrams, formulas, and one-click Word export. Learn more at https://docu.md
---

# IoT Architecture Diagram Generator

**Quick Start:** Select device/sensor icons → Place edge gateways → Connect to cloud services → Group into zones → Wrap in ` ```plantuml ` fence.

> ⚠️ **IMPORTANT:** Always use ` ```plantuml ` or ` ```puml ` code fence. NEVER use ` ```text ` — it will NOT render as a diagram.

## Critical Rules

- Every diagram starts with `@startuml` and ends with `@enduml`
- Use `left to right direction` for typical IoT data flows (Device → Edge → Cloud)
- Use `mxgraph.aws4.*` stencil syntax for IoT service and device icons
- Default colors are applied automatically — you do NOT need to specify `fillColor` or `strokeColor`
- Use `rectangle "Zone"  { ... }` or `package "Site" { ... }` for grouping
- Directed flows u
```

</details>
