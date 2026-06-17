---
name: nyaggah__bedframe__skill
source: https://github.com/nyaggah/bedframe/blob/f564e7285b3ca4ad2816c73884ecc582f1d24482/packages/skills/bedframe/SKILL.md
repo: nyaggah/bedframe
kind: skill
stars: 582
last_pushed: 2026-06-08T16:36:35Z
license: mit
score: 9
domains: [web-extensions, cli-tools, development-frameworks]
tags: [browser-extension, framework-specific, structured-routing]
curated: 2026-06-15
curated_by: config-scout
---

# nyaggah/bedframe — skill

**Why it's worth keeping:** The 'Operating Model' uses a high-density routing pattern that teaches the agent how to navigate specialized reference documentation rather than bloating the prompt. The 'Critical Rules' section provides essential constraints that prevent common mistakes like editing generated build artifacts.

**Summary:** This skill defines a project-specific operating model for the Bedframe browser extension framework. It establishes canonical sources of truth and provides task-based routing instructions.

**Source credibility:** High; 582 stars and recent activity indicate a mature, well-maintained framework.

**Recency:** Very current; it utilizes advanced structured routing techniques ideal for modern agentic workflows.

**Source:** [nyaggah/bedframe/packages/skills/bedframe/SKILL.md](https://github.com/nyaggah/bedframe/blob/f564e7285b3ca4ad2816c73884ecc582f1d24482/packages/skills/bedframe/SKILL.md) · 582★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bedframe
description: Work in a Bedframe browser extension project. Use when the repository contains AGENTS.md, src/_config/bedframe.config.ts, src/manifests/*, or the task involves the Bedframe CLI, @bedframe/core, browser manifests, extension pages, Vite config, or release flow.
---

# Bedframe

Use this skill for any task inside a Bedframe project.

Bedframe is a cross-browser browser extension framework built around the `B.E.D.` model:

- `Browser`
- `Extension`
- `Development`

Most project-defining changes should be understood through `src/_config/bedframe.config.ts` and the root `AGENTS.md`.

## Inspect first

- `AGENTS.md`
- the nearest folder-level `AGENTS.md` for the files you are editing
- `src/_config/bedframe.config.ts`

## Critical rules

- Treat `src/_config/bedframe.config.ts` as the canonical project definition.
- Keep config, manifests, pages, scripts, package metadata, and workflow files aligned.
- Edit source files, not generated `dist/*` output.
- Use `@bedframe/core` helpers and types when they already define the structure.
- Use the smallest Bedframe CLI command that verifies the task.
- Treat build support and publish support as different concerns.
```

</details>
