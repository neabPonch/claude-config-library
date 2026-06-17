---
name: mattnigh__skills_collection__gocallum-nextjs16-agent-skills-claude-skills-nextjs16-skills-skill-md
source: https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/gocallum__nextjs16-agent-skills__claude__skills__nextjs16-skills__SKILL.MD
repo: mattnigh/skills_collection
kind: skill
stars: 23
last_pushed: 2025-12-31T03:21:29Z
license: unknown
score: 9
domains: [web-frontend, javascript, react]
tags: [nextjs, upgrade-guide, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# mattnigh/skills_collection — skill

**Why it's worth keeping:** It captures critical 'gotchas' like the shift to asynchronous request APIs (params/searchParams) which are frequent failure points for LLMs.

**Summary:** A high-density technical reference for Next.js evolution, focusing on breaking changes, upgrade paths, and configuration shifts.

**Source credibility:** High-quality technical detail likely curated by a developer tracking Next.js canary/experimental features.

**Recency:** Highly current, focusing on modern React/Next.js architectural shifts.

**Source:** [mattnigh/skills_collection/collection/gocallum__nextjs16-agent-skills__claude__skills__nextjs16-skills__SKILL.MD](https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/gocallum__nextjs16-agent-skills__claude__skills__nextjs16-skills__SKILL.MD) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nextjs16-skills
description: Key facts and links for Next.js 16. Use for planning, writing, and troubleshooting Next.js 16 changes.
---

## Links

- Docs: https://nextjs.org/docs
- Upgrade guide (v16): https://nextjs.org/docs/app/guides/upgrading/version-16
- Release notes/blog: https://nextjs.org/blog/next-16

## Upgrade

```sh
# Automated upgrade
npx @next/codemod@canary upgrade latest

# Manual upgrade
npm install next@latest react@latest react-dom@latest

# New project
npx create-next-app@latest
```

Codemod covers (high-level): moves Turbopack config, migrates `next lint` → ESLint CLI, migrates `middleware` → `proxy`, removes some `unstable_` prefixes, removes route-level `experimental_ppr`.

TypeScript: also upgrade `@types/react` and `@types/react-dom`.

## What’s New (v16)

- Cache Components: opt-in caching via the `"use cache"` directive; evolves/absorbs PPR.
- Next.js DevTools MCP: Model Context Protocol integration for AI-assisted debugging.
- `proxy.ts`: clearer network boundary; `middleware.ts` deprecated for most use.
- Better logs/metrics: more detailed `next dev` and build timing output.

## Performance / DX

- Turbopack: stable; default bundler (opt out
```

</details>
