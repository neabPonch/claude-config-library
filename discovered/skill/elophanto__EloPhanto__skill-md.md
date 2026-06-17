---
name: elophanto__EloPhanto__skill-md
source: https://github.com/elophanto/EloPhanto/blob/d31c2204f80bb0d864a901e830df14bf28c5233d/skills/nextjs/SKILL.MD
repo: elophanto/EloPhanto
kind: skill
stars: 78
last_pushed: 2026-06-03T05:54:03Z
license: apache-2.0
score: 9
domains: [web-frontend, javascript-frameworks]
tags: [nextjs, react, typescript, migration]
curated: 2026-06-15
curated_by: config-scout
---

# elophanto/EloPhanto — skill

**Why it's worth keeping:** The inclusion of a 'Verify' checklist gives the agent specific validation steps to ensure code quality after an operation. It also focuses on high-impact breaking changes like async Request APIs which prevent common hallucination errors.

**Summary:** A highly technical reference for Next.js 16 that covers breaking changes, configuration migrations, and API updates.

**Source credibility:** High-quality, highly detailed documentation from a specialized autonomous agent repository.

**Recency:** Very recent; targets cutting-edge Next.js features and patterns.

**Source:** [elophanto/EloPhanto/skills/nextjs/SKILL.MD](https://github.com/elophanto/EloPhanto/blob/d31c2204f80bb0d864a901e830df14bf28c5233d/skills/nextjs/SKILL.MD) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nextjs16-skills
description: Key facts and links for Next.js 16. Use for planning, writing, and troubleshooting Next.js 16 changes.
---


## Triggers

- nextjs
- next.js
- next
- app router
- server component
- ssr
- ssg
- vercel
- next 16
- pages router
- middleware
- next api

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
- `proxy.ts`: clearer network boundary; `middleware.ts` deprecated for most use
```

</details>
