---
name: remeda__remeda__skill
source: https://github.com/remeda/remeda/blob/a80d3158cd75e824a59a5522b14217c769d8f6e0/.agents/skills/shadcn-add/SKILL.md
repo: remeda/remeda
kind: skill
stars: 5379
last_pushed: 2026-06-14T12:24:43Z
license: mit
score: 8
domains: [web-frontend, react, tailwind-css]
tags: [refactoring, shadcn, cleanup, modernization]
curated: 2026-06-15
curated_by: config-scout
---

# remeda/remeda — skill

**Why it's worth keeping:** It defines specific, actionable refactoring rules (import stripping, directive removal) that turn a manual post-CLI chore into an automated skill. The focus on Tailwind v4 modernization makes it highly future-proof.

**Summary:** Automates the cleanup of shadcn-generated components to align with modern React practices and Tailwind v4 standards.

**Source credibility:** High quality; demonstrates deep knowledge of modern frontend build-tooling transitions.

**Recency:** Highly current, specifically addressing Tailwind v4 and modern React import patterns.

**Source:** [remeda/remeda/.agents/skills/shadcn-add/SKILL.md](https://github.com/remeda/remeda/blob/a80d3158cd75e824a59a5522b14217c769d8f6e0/.agents/skills/shadcn-add/SKILL.md) · 5379★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: shadcn-add
description: Follow up cleanup and refactors that **must** be done whenever a new shadcn component is added via the add cli command. This skill should be checked whenever a new file is added to the shadcn ui component directory (`src/components/ui`).
---

# Remove:

- The global React namespace import (`import * as React from "react"`); only import the concrete types and utilities needed.
- Any `React.` prefixes, both in types and in runtime code.
- The global `export { }` block; add the export keyword to each declaration instead.
- `"use client"` directives.
- Blank lines within the import statements.

# Fix:

- Issues caused by having `exactOptionalPropertyTypes` enabled. This might require removing props from destructurings.
- Tailwind v4 modernization concerns (squashing `data-['xxx']` attributes to `data-xxx`, converting arbitrary sizes to concrete values, e.g. `size-[3rem]` to `size-12`).

# Organize:

- Sort imports via the vscode "Organize Imports" source action.
```

</details>
