---
name: 4gray__iptvnator__skill
source: https://github.com/4gray/iptvnator/blob/3d2549dacea5c98239eb8aab6c3acd494878fef5/.codex/skills/iptvnator-nx-architecture/SKILL.md
repo: 4gray/iptvnator
kind: skill
stars: 6237
last_pushed: 2026-06-14T21:58:15Z
license: mit
score: 8
domains: [web-frontend, monorepo-management, architecture]
tags: [nx, monorepo, typescript, governance]
curated: 2026-06-15
curated_by: config-scout
---

# 4gray/iptvnator — skill

**Why it's worth keeping:** Provides clear governance for dependency direction via specific tag families (type:ui vs type:data-access) and enforces scoped alias usage over legacy imports.

**Summary:** Defines the Nx monorepo structure, import aliasing rules, and project tagging conventions to maintain architectural boundaries.

**Source credibility:** Highly credible; source is a well-starred, actively maintained open-source project.

**Recency:** 

**Source:** [4gray/iptvnator/.codex/skills/iptvnator-nx-architecture/SKILL.md](https://github.com/4gray/iptvnator/blob/3d2549dacea5c98239eb8aab6c3acd494878fef5/.codex/skills/iptvnator-nx-architecture/SKILL.md) · 6237★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: iptvnator-nx-architecture
description: Repository-specific Nx monorepo structure, library placement rules, scoped path aliases, and migration guardrails for portal/workspace/app code.
---

# IPTVnator Nx Architecture

Use this skill when deciding where code belongs, extracting libraries, changing imports, editing project tags, or refactoring portal/workspace/app boundaries.

## Project Shape

- `apps/web`: Angular renderer application.
- `apps/electron-backend`: Electron main process and native/runtime integration.
- `apps/*-e2e`: Playwright E2E projects.
- `apps/*-mock-server`: local development and E2E mock servers.
- `libs/playlist/*`: M3U/import/shared playlist functionality.
- `libs/portal/*`: Xtream, Stalker, and provider-neutral portal functionality.
- `libs/workspace/*`: workspace shell and dashboard.
- `libs/ui/*`: provider-neutral UI, playback, EPG, remote control, and pipes.
- `libs/shared/*`: contracts, database, and pure utility code.

## Import Policy

- Use scoped aliases from `tsconfig.base.json`, for example `@iptvnator/services` and `@iptvnator/shared/interfaces`.
- Do not reintroduce legacy bare aliases such as `services`, `components`, or `shared-inter
```

</details>
