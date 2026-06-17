---
name: dcaslin__d2-checklist
source: https://github.com/dcaslin/d2-checklist/blob/4824dc8a08b8e2a9bea7f087410569013d91d738/CLAUDE.md
repo: dcaslin/d2-checklist
kind: claude-md
stars: 93
last_pushed: 2026-06-11T02:12:41Z
license: mit
score: 9
domains: [web-frontend, angular]
tags: [angular, environment-setup, tribal-knowledge]
curated: 2026-06-15
curated_by: config-scout
---

# dcaslin/d2-checklist — claude-md

**Why it's worth keeping:** Contains high-value 'tribal knowledge' about how scripts affect package.json and explicit rules on when to deviate from standard linting practices (console logs).

**Summary:** Provides critical setup instructions for gitignored environment files and specific build-time side effects involving the Bungie manifest. It also outlines architectural patterns and unique development constraints.

**Source credibility:** High; active repository with specific domain requirements and clear developer workflows.

**Recency:** Highly current, referencing modern Angular 19 standards.

**Source:** [dcaslin/d2-checklist/CLAUDE.md](https://github.com/dcaslin/d2-checklist/blob/4824dc8a08b8e2a9bea7f087410569013d91d738/CLAUDE.md) · 93★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project overview

d2-checklist is the Angular front end for [d2checklist.com](https://www.d2checklist.com), a Destiny 2 companion app. It uses Angular 19, Angular Material, and the Bungie API.

## Build and run

```bash
npm install          # install dependencies
npm start            # serves on https://localhost:4200
npm run build        # development build
npm run build:prod   # production build
npm run lint         # eslint
```

## IMPORTANT NOTES

ALWAYS bump the version in package.json for each new PR. If the bungie manifest version changes, also bump package.json's "manifest" value. These two values are used to bust caches on browser clients, if not bumped the clients won't see the new values.

New workspaces/worktrees are missing the gitignored `src/environments/keys.ts` and `keys-prod.ts` (Bungie API credentials), so builds and tests fail with "Cannot find module './keys'". Copy them from the base checkout:

```bash
cp ~/projects/d2-checklist/src/environments/keys.ts ~/projects/d2-checklist/src/environments/keys-prod.ts src/environments/
```

New workspaces are also missing node_modules and the gitignored manifest JSON in `src/assets/` (`destiny2-*.json`), s
```

</details>
