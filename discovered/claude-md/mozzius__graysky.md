---
name: mozzius__graysky
source: https://github.com/mozzius/graysky/blob/abef3e4859955fdf5b02d67b478e769003352cd6/CLAUDE.md
repo: mozzius/graysky
kind: claude-md
stars: 673
last_pushed: 2026-01-07T16:12:45Z
license: mit
score: 8
domains: [mobile-app, fullstack-web, monorepo]
tags: [react-native, nextjs, turborepo, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# mozzius/graysky — claude-md

**Why it's worth keeping:** It explicitly maps internal package dependencies and provides precise command sets for specialized tasks across the entire stack. The inclusion of strict coding conventions and database schemas makes it highly actionable for an agent.

**Summary:** A comprehensive technical blueprint for a full-stack monorepo containing mobile (Expo) and web (Next.js) clients.

**Source credibility:** High: established open-source project with significant stars and recent activity.

**Recency:** Very current; uses cutting-edge versions like Next.js 16 and Tailwind 4.

**Source:** [mozzius/graysky/CLAUDE.md](https://github.com/mozzius/graysky/blob/abef3e4859955fdf5b02d67b478e769003352cd6/CLAUDE.md) · 673★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Graysky - Bluesky Client Monorepo

A full-stack Bluesky client with React Native mobile app, Next.js web app, and push notification service.

## Quick Commands

```bash
pnpm dev           # Start Expo mobile app
pnpm dev:both      # Start Expo + Next.js in parallel
pnpm dev:next      # Start Next.js web app only
pnpm dev:push      # Start push notification service
pnpm lint          # Run ESLint across all packages
pnpm format:fix    # Run Prettier formatting
pnpm typecheck     # TypeScript type checking
pnpm db:generate   # Generate Prisma client
pnpm db:push       # Push Prisma schema to database
```

## Project Structure

```
apps/
  expo/          # React Native mobile app (Expo 54, RN 0.81, React 19)
  nextjs/        # Next.js 16 web app (marketing/web presence)
  push-notifs/   # Backend push notification service

packages/
  api/           # tRPC router (shared API layer)
  db/            # Prisma database client and schema

tooling/
  eslint/        # Shared ESLint configs (flat config format)
  prettier/      # Shared Prettier config
  tailwind/      # Shared Tailwind config
  typescript/    # Base TypeScript config
```

## Key Technologies

- **Mobile**: Expo 54, React
```

</details>
