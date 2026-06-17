---
name: Arize-ai__phoenix__skill
source: https://github.com/Arize-ai/phoenix/blob/bb17922331af5231f33c73e574a34b0bf39de315/.agents/skills/phoenix-typescript-package-docs/SKILL.md
repo: Arize-ai/phoenix
kind: skill
stars: 10167
last_pushed: 2026-06-17T01:41:21Z
license: other
score: 9
domains: [documentation, typescript, devops]
tags: [docs-sync, npm-lifecycle, api-maintenance]
curated: 2026-06-17
curated_by: config-scout
---

# Arize-ai/phoenix — skill

**Why it's worth keeping:** It provides high-leverage techniques like mapping 'Source of Truth' vs. 'Generated Artifacts', mandatory verification using `npm pack --dry-run`, and specific rules to prevent API drift by grounding docs in actual code exports.

**Summary:** A procedural skill file that manages a complex synchronization flow between canonical Mintlify documentation and distributed npm package exports.

**Source credibility:** High; maintained by Arize AI, a prominent player in the AI observability space.

**Recency:** Current; uses modern npm lifecycle patterns and contemporary TypeScript workflows.

**Source:** [Arize-ai/phoenix/.agents/skills/phoenix-typescript-package-docs/SKILL.md](https://github.com/Arize-ai/phoenix/blob/bb17922331af5231f33c73e574a34b0bf39de315/.agents/skills/phoenix-typescript-package-docs/SKILL.md) · 10167★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: phoenix-typescript-package-docs
description: >
  Maintain the bundled TypeScript package docs that ship inside Phoenix npm packages.
  Use this skill whenever adding or updating docs for `@arizeai/phoenix-client`,
  `@arizeai/phoenix-evals`, or `@arizeai/phoenix-otel`, when changing the Mintlify
  package-doc pages, when keeping `node_modules/.../docs` content aligned with actual
  exports, or when modifying the sync and publish flow for packaged docs.
license: Apache-2.0
metadata:
  author: oss@arize.com
  version: "1.0.0"
  languages: TypeScript
  internal: true
---

# Phoenix TypeScript Package Docs

Keep the curated TypeScript package docs aligned with the real npm package surface area and with the publish-time sync flow.

## Quick Reference

| Task | What to inspect | What to update |
| ----- | ----- | ----- |
| Fix a stale example | `js/packages/<pkg>/src/` exports and function signatures | Canonical MDX under `docs/phoenix/sdk-api-reference/typescript/packages/<pkg>/` |
| Add or remove a page | Existing package-doc folder and `docs.json` nav | Canonical MDX, `docs.json`, and any landing-page links |
| Add a new package to the bundled-docs system | `js/scripts/sync-
```

</details>
