---
name: rrh1441__remotion-ui
source: https://github.com/rrh1441/remotion-ui/blob/b3739f8a4034c1c3a4def3f3cf025f11efe43442/claude.md
repo: rrh1441/remotion-ui
kind: claude-md
stars: 9
last_pushed: 2025-09-02T21:07:43Z
license: unknown
score: 9
domains: [cli-tools, frontend-architecture, component-libraries]
tags: [system-design, technical-spec, monorepo]
curated: 2026-06-14
curated_by: config-scout
---

# rrh1441/remotion-ui — claude-md

**Why it's worth keeping:** It demonstrates how to define strict data schemas (asset manifests), precise CLI command behaviors, and complex monorepo architectures to ensure a cohesive ecosystem rather than isolated files.

**Summary:** A high-fidelity technical specification designed to guide an agent through the end-to-end construction of a component library, CLI, and asset system.

**Source credibility:** Niche repository with highly professional-grade technical specifications.

**Recency:** 

**Source:** [rrh1441/remotion-ui/claude.md](https://github.com/rrh1441/remotion-ui/blob/b3739f8a4034c1c3a4def3f3cf025f11efe43442/claude.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Below is a **single, comprehensive prompt** you can hand to an autonomous agent. It defines scope, deliverables, directory trees, APIs, code standards, tests, and acceptance criteria for building a “shadcn for Remotion” with an ambitious v0.1 asset set.

---

# PROMPT FOR AGENT

## Mission

Build **Remotion-UI**, a **source-first** component, asset, and preset system for Remotion (think “shadcn for motion”). Deliver a copy-in **CLI** that installs TypeScript components, aspect-ratio presets with safe-areas, and versioned asset packs (icons, characters, shapes, backgrounds) into any Remotion project. Provide optional runtime packages and an eject path.

## Success Criteria (Definition of Done)

1. **CLI** (`@remotion-ui/cli`) publishes to npm and supports:

   * `init` (tokens, ThemeProvider, presets, Tailwind mapping optional)
   * `add <components...>` (copy TSX files)
   * `add assets <packs...>` (copy `/public/assets` + `manifest.json`)
   * `add-preset <ids...>` (scaffold demo compositions)
   * Idempotent, safe, lint-clean output. No TODOs.
2. **Components & primitives** compile in a fresh Remotion app with zero type or lint errors and render correctly.
3. **Assets**: v0.1 shi
```

</details>
