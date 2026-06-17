---
name: elophanto__EloPhanto__skill
source: https://github.com/elophanto/EloPhanto/blob/d31c2204f80bb0d864a901e830df14bf28c5233d/skills/swiftui-ui-patterns/SKILL.md
repo: elophanto/EloPhanto
kind: skill
stars: 78
last_pushed: 2026-06-03T05:54:03Z
license: apache-2.0
score: 8
domains: [mobile, ios, swiftui]
tags: [ui-patterns, apple-ecosystem]
curated: 2026-06-15
curated_by: config-scout
---

# elophanto/EloPhanto — skill

**Why it's worth keeping:** The 'Sheet owns its actions' pattern prevents callback-driven architecture, while the 'Verify' section provides actionable QA steps like checking dark mode and accessibility.

**Summary:** Provides architectural standards for SwiftUI development including state management, component composition, and sheet patterns. Includes a rigorous verification checklist for quality assurance.

**Source credibility:** High-quality documentation from an active/recent autonomous agent repository.

**Recency:** Current; utilizes modern SwiftUI patterns such as @Observable and async/await.

**Source:** [elophanto/EloPhanto/skills/swiftui-ui-patterns/SKILL.md](https://github.com/elophanto/EloPhanto/blob/d31c2204f80bb0d864a901e830df14bf28c5233d/skills/swiftui-ui-patterns/SKILL.md) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: swiftui-ui-patterns
description: Best practices and example-driven guidance for building SwiftUI views and components. Use when creating or refactoring SwiftUI UI, designing tab architecture with TabView, composing screens, or needing component-specific patterns and examples.
---

# SwiftUI UI Patterns


## Triggers

- swiftui
- swift
- ios
- macos
- apple
- xcode
- swift ui
- ios app
- mac app
- watchos
- tvos
- swift view
- modifier

## Quick start

Choose a track based on your goal:

### Existing project

- Identify the feature or screen and the primary interaction model (list, detail, editor, settings, tabbed).
- Find a nearby example in the repo with `rg "TabView\("` or similar, then read the closest SwiftUI view.
- Apply local conventions: prefer SwiftUI-native state, keep state local when possible, and use environment injection for shared dependencies.
- Choose the relevant component reference from `references/components-index.md` and follow its guidance.
- Build the view with small, focused subviews and SwiftUI-native data flow.

### New project scaffolding

- Start with `references/app-scaffolding-wiring.md` to wire TabView + NavigationStack + sheets.
- Add a min
```

</details>
