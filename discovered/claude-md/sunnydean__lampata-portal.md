---
name: sunnydean__lampata-portal
source: https://github.com/sunnydean/lampata-portal/blob/730fdfd7c67dc7134d22fc74970c4d79ae0ba3c6/CLAUDE.md
repo: sunnydean/lampata-portal
kind: claude-md
stars: 0
last_pushed: 2026-05-30T18:00:12Z
license: unknown
score: 8
domains: [web-frontend, security]
tags: [react, tailwind-v4, docker, vite]
curated: 2026-06-14
curated_by: config-scout
---

# sunnydean/lampata-portal — claude-md

**Why it's worth keeping:** Uses effective 'edit-this-not-that' constraints (e.g., update siteContent.ts instead of components) to prevent the AI from creating hardcoded technical debt.

**Summary:** Provides highly specific operational commands for secure Dockerized development and a clear structural map of content vs. component logic.

**Source credibility:** Low reputation/stars, but the high level of specificity suggests a manually authored, professional-grade configuration.

**Recency:** Extremely current; uses modern tool versions like Tailwind v4 and Node 22.

**Source:** [sunnydean/lampata-portal/CLAUDE.md](https://github.com/sunnydean/lampata-portal/blob/730fdfd7c67dc7134d22fc74970c4d79ae0ba3c6/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
docker compose -f compose.safe.yaml up --build app
docker compose -f compose.safe.yaml run --rm app sh -lc "pnpm install --frozen-lockfile --store-dir /pnpm/store && pnpm run build"
docker compose -f compose.safe.yaml down --volumes --remove-orphans

pnpm install       # install dependencies
pnpm run dev       # start Vite dev server
pnpm run security  # locked package age check, advisory audit, and registry signature verification
pnpm run build     # security checks, then production build
```

Prefer the Docker sandbox for local development when reducing host exposure to compromised packages matters. It does not mount the host home directory; dependency installs, cache, and pnpm store live in Docker volumes.

pnpm is configured in `pnpm-workspace.yaml` to block install/build lifecycle scripts, verify registry signatures, require packages to be at least 10 days old before resolution, fail on stale dependency state before scripts run, and pin newly added dependencies exactly.
This project uses `pnpm@11.0.4`, which requires Node.js 22.13 or newer.
```

</details>
