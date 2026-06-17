---
name: WelcometoMyGarden__welcometomygarden
source: https://github.com/WelcometoMyGarden/welcometomygarden/blob/21c85e879fba4cb3dfb3241b9d580fe1dc5648b4/CLAUDE.md
repo: WelcometoMyGarden/welcometomygarden
kind: claude-md
stars: 117
last_pushed: 2026-06-16T15:10:15Z
license: agpl-3.0
score: 9
domains: [web-frontend, backend-api]
tags: [sveltekit, firebase, fullstack]
curated: 2026-06-16
curated_by: config-scout
---

# WelcometoMyGarden/welcometomygarden — claude-md

**Why it's worth keeping:** It proactively identifies specific logic pitfalls (like auth state transitions) and provides the necessary environment variables required to run local emulators without error.

**Summary:** Provides deep architectural context, command patterns, and critical logic edge cases for a SvelteKit/Firebase stack.

**Source credibility:** Active repository with high-quality technical documentation and modern toolchain usage.

**Recency:** Extremely current, referencing Node 24 and recent development activity.

**Source:** [WelcometoMyGarden/welcometomygarden/CLAUDE.md](https://github.com/WelcometoMyGarden/welcometomygarden/blob/21c85e879fba4cb3dfb3241b9d580fe1dc5648b4/CLAUDE.md) · 117★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with code in this repository.

## About

Welcome To My Garden (WTMG) is a platform connecting slow travelers with hosts who offer free camping spots in their gardens. The codebase is a SvelteKit frontend with Firebase backend (Firestore, Auth, Cloud Functions) and a Supabase PostgreSQL replica for advanced queries.

### Superfan and Membership

To use many core WTMG features, users need to be a "member". This was previously called "superfan", and is technically still referred to as "superfan" in many code areas (i18n). For new features or fixes, we should aim to use the term "member" or "membership".

Users can host their garden without being a member.

To check is user is a member, check the `$user.superfan` boolean.

## Commands

### Frontend

```bash
yarn dev                   # Start dev server (against local emulators)
yarn dev:staging           # Dev server against staging backend
yarn build                 # Production build
yarn check                 # TypeScript + svelte-check (type checking)
yarn check:watch           # Watch mode
yarn lint                  # ESLint + Prettier check
yarn format
```

</details>
