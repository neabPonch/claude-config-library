---
name: simular-ai__simulang
source: https://github.com/simular-ai/simulang/blob/d37e3f41a1c92f9da8b0fb6f3667a39c274999cf/SKILL.md
repo: simular-ai/simulang
kind: skill
stars: 127
last_pushed: 2026-06-15T03:25:12Z
license: mit
score: 9
domains: [cli-tools, desktop-automation, typescript]
tags: [automation, macos, developer-tools]
curated: 2026-06-15
curated_by: config-scout
---

# simular-ai/simulang — skill

**Why it's worth keeping:** The 'API Discovery' section provides an elite strategy by instructing the agent to use `simulang which` to find local type definitions/docs for a specific version, preventing hallucinations. It also includes critical runtime pitfalls regarding accessibility trees and enum mapping.

**Summary:** Provides specialized context for the simulang desktop automation CLI and its TypeScript library.

**Source credibility:** High; derived from an active, specialized automation tool repository.

**Recency:** Very current; references modern Node.js versions and contemporary macOS permission workflows.

**Source:** [simular-ai/simulang/SKILL.md](https://github.com/simular-ai/simulang/blob/d37e3f41a1c92f9da8b0fb6f3667a39c274999cf/SKILL.md) · 127★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: simulang
description: |
  Use when working with simulang scripts (typically .ts or .mts), the simulang
  CLI, or @simular-ai/simulang-js (Node bindings for the simulang-rs desktop
  automation crate). Covers how to write, run, and debug scripts, how to look
  up the simulang-js API, and the per-script version-pin model.
---

# simulang

`simulang` is the CLI that runs TypeScript or JavaScript scripts against the
`@simular-ai/simulang-js` desktop-automation library. It bundles its own copy
of simulang-js but lets each script pin a specific version.

## When to use this skill

- The user is editing or running a file with extension `.ts`, `.mts`, `.js`,
  `.mjs`, or `.simulang` that imports `@simular-ai/simulang-js`.
- The user mentions `simulang` (the CLI) or `simulang-js`, or
  desktop automation tasks (mouse, keyboard, screenshots, app launching,
  accessibility trees).
- The user wants to write a new script for desktop automation.

## First-time setup / troubleshooting permissions

Run `simulang setup` once after installing (and again any time screenshots,
accessibility, or mouse control stop working). It grants the macOS permissions
— Screen Recording, Accessibility, an
```

</details>
