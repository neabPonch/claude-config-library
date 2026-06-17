---
name: alamenai__terrae
source: https://github.com/alamenai/terrae/blob/ea9a4803463817393c1da6ce486e42ebd7eac341/CLAUDE.md
repo: alamenai/terrae
kind: claude-md
stars: 233
last_pushed: 2026-04-06T16:43:28Z
license: mit
score: 8
domains: [web-frontend, ui-components]
tags: [modular-rules, gotchas, react, nextjs]
curated: 2026-06-15
curated_by: config-scout
---

# alamenai/terrae — claude-md

**Why it's worth keeping:** The separation of rules into domain-specific files prevents context bloat, while the 'Project Gotchas' section provides high-signal instructions for specific framework behaviors like Mapbox/Next.js context requirements.

**Summary:** Uses a highly modular rule system and emphasizes critical runtime 'gotchas' that prevent breaking changes.

**Source credibility:** Solid; 233 stars suggests a real-world component library used by others.

**Recency:** Highly current; last pushed 2 months ago and follows modern modular documentation patterns.

**Source:** [alamenai/terrae/CLAUDE.md](https://github.com/alamenai/terrae/blob/ea9a4803463817393c1da6ce486e42ebd7eac341/CLAUDE.md) · 233★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
@.claude/rules/overview.md
@.claude/rules/typescript.md
@.claude/rules/javascript.md
@.claude/rules/react.md
@.claude/rules/nextjs.md
@.claude/rules/security.md
@.claude/rules/clean-code.md

# Common Commands

- `npm run dev` - Start Next.js dev server
- `npm run build` - Production build
- `npm run lint` - Run ESLint
- `npm run format` - Format with Prettier
- `npm run format:check` - Check formatting
- `npm run test:run` - Run tests once
- `npm run test:coverage` - Run tests with coverage
- `npm run registry:build` - Build component registry to `./public`
- `npx tsc --noEmit` - Type-check without emitting

# Project Gotchas

- Mapbox GL requires `"use client"` on all map components
- The `useMap()` hook only works inside the `<Map>` provider context
- Always check `isLoaded` from `useMap()` before accessing the map instance
- Registry components are installed into user projects, so never include side effects beyond the component's purpose
- Husky pre-commit hook runs `npm run build` and will fail the commit if the build breaks
- Commit messages must follow conventional commits format (enforced by commitlint)
- Do not add `Co-Authored-By` lines to commit messages
- Do not commit u
```

</details>
