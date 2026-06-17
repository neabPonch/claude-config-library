---
name: Comfy-Org__ComfyUI_frontend__skill
source: https://github.com/Comfy-Org/ComfyUI_frontend/blob/2b0bcda41fef5ad06d1ccfdea407cbbeb7661a31/.claude/skills/layer-audit/SKILL.md
repo: Comfy-Org/ComfyUI_frontend
kind: skill
stars: 1845
last_pushed: 2026-06-15T03:58:53Z
license: gpl-3.0
score: 8
domains: [web-frontend, architecture]
tags: [eslint, architecture, linting, layering]
curated: 2026-06-15
curated_by: config-scout
---

# Comfy-Org/ComfyUI_frontend — skill

**Why it's worth keeping:** Provides specific CLI patterns for targeted error detection and offers clear 'Resolution Strategies' that guide an agent through structural refactoring.

**Summary:** Defines a protocol for detecting and enforcing a strict four-layer architectural hierarchy using ESLint.

**Source credibility:** High; part of the highly-starred ComfyUI frontend repository with recent maintenance.

**Recency:** 

**Source:** [Comfy-Org/ComfyUI_frontend/.claude/skills/layer-audit/SKILL.md](https://github.com/Comfy-Org/ComfyUI_frontend/blob/2b0bcda41fef5ad06d1ccfdea407cbbeb7661a31/.claude/skills/layer-audit/SKILL.md) · 1845★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: layer-audit
description: 'Detect violations of the layered architecture import rules (base -> platform -> workbench -> renderer). Runs ESLint with the import-x/no-restricted-paths rule and generates a grouped report.'
---

# Layer Architecture Audit

Finds imports that violate the layered architecture boundary rules enforced by `import-x/no-restricted-paths` in `eslint.config.ts`.

## Layer Hierarchy (bottom to top)

```
renderer  (top -- can import from all lower layers)
   ^
workbench
   ^
platform
   ^
  base    (bottom -- cannot import from any upper layer)
```

Each layer may only import from layers below it.

## How to Run

```bash
# Run ESLint filtering for just the layer boundary rule violations
pnpm lint 2>&1 | grep 'import-x/no-restricted-paths' -B1 | head -200
```

To get a full structured report, run:

```bash
# Collect all violations from base/, platform/, workbench/ layers
pnpm eslint src/base/ src/platform/ src/workbench/ --no-error-on-unmatched-pattern --rule '{"import-x/no-restricted-paths": "warn"}' --format compact 2>&1 | grep 'no-restricted-paths' | sort
```

## How to Read Results

Each violation line shows:

- The **file** containing the bad import
-
```

</details>
