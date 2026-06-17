---
name: oyjt__uniapp-vue3-template__skill
source: https://github.com/oyjt/uniapp-vue3-template/blob/4d7f3075a739c37c7fd7cff73a5d2ee7d034e113/.trae/skills/antfu/SKILL.md
repo: oyjt/uniapp-vue3-template
kind: skill
stars: 621
last_pushed: 2026-06-04T08:15:50Z
license: mit
score: 9
domains: [web-frontend, tooling]
tags: [vue, typescript, pnpm, vitest, opinionated]
curated: 2026-06-16
curated_by: config-scout
---

# oyjt/uniapp-vue3-template — skill

**Why it's worth keeping:** Provides specific CLI command mappings (via @antfu/ni), strict TypeScript configurations, and precise file structuring for testing and documentation that an agent can execute without ambiguity.

**Summary:** A highly opinionated development standard centered on Anthony Fu's expert-level web tooling and best practices.

**Source credibility:** Extremely high; the profile follows the standards of a prominent ecosystem leader in Vue and Vite.

**Recency:** Very current, utilizing modern ESM-first patterns and latest pnpm features.

**Source:** [oyjt/uniapp-vue3-template/.trae/skills/antfu/SKILL.md](https://github.com/oyjt/uniapp-vue3-template/blob/4d7f3075a739c37c7fd7cff73a5d2ee7d034e113/.trae/skills/antfu/SKILL.md) · 621★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: antfu
description: Anthony Fu's {Opinionated} preferences and best practices for web development
metadata:
  author: Anthony Fu
  version: "2026.1.28"
---

# Anthony Fu's Preferences

This skill covers Anthony Fu's preferred tooling, configurations, and best practices for web development. This skill is opinionated.

## Quick Summary

| Category | Preference |
|----------|------------|
| Package Manager | pnpm |
| Language | TypeScript (strict mode) |
| Module System | ESM (`"type": "module"`) |
| Linting & Formatting | @antfu/eslint-config (no Prettier) |
| Testing | Vitest |
| Git Hooks | simple-git-hooks + lint-staged |
| Documentation | VitePress (in `docs/`) |

---

## Core Stack

### Package Manager (pnpm)

Use pnpm as the package manager.

For monorepo setups, use pnpm workspaces:

```yaml
# pnpm-workspace.yaml
packages:
  - 'packages/*'
```


Use pnpm named catalogs in `pnpm-workspace.yaml` to manage dependency versions:

| Catalog | Purpose |
|---------|---------|
| `prod` | Production dependencies |
| `inlined` | Dependencies inlined by bundler |
| `dev` | Development tools (linter, bundler, testing, dev-server) |
| `frontend` | Frontend libraries bundled into fr
```

</details>
