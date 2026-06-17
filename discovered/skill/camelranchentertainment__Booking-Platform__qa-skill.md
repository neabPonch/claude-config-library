---
name: camelranchentertainment__Booking-Platform__qa-skill
source: https://github.com/camelranchentertainment/Booking-Platform/blob/7db9654012eceb2a5a37bd7de2fd18ecbde51f0b/QA_SKILL.md
repo: camelranchentertainment/Booking-Platform
kind: skill
stars: 0
last_pushed: 2026-06-16T20:32:23Z
license: unknown
score: 8
domains: [web-frontend, security, qa-automation]
tags: [qa, audit, nextjs, security]
curated: 2026-06-16
curated_by: config-scout
---

# camelranchentertainment/Booking-Platform — skill

**Why it's worth keeping:** It provides a blueprint for using grep/find to enforce architectural invariants (like mandatory auth checks) rather than just running existing tests.

**Summary:** A command-driven QA audit skill that uses shell patterns to verify routing, auth guards, API security, and business logic integrity.

**Source credibility:** Low social proof (0 stars), but demonstrates high-level engineering intent.

**Recency:** Current; utilizes standard Unix primitives perfectly suited for terminal-based agent tool use.

**Source:** [camelranchentertainment/Booking-Platform/QA_SKILL.md](https://github.com/camelranchentertainment/Booking-Platform/blob/7db9654012eceb2a5a37bd7de2fd18ecbde51f0b/QA_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gstack-qa
description: Full visual and functional QA audit of a Next.js web platform. Use this skill when asked to run /qa, perform a QA audit, or visually verify the platform works correctly. Systematically checks every page, every route, every interactive element, and every data flow. Reports all issues with severity ratings and fixes what it can automatically.
---

# GStack /qa — Full Platform QA Skill

You are acting as a QA engineer performing a comprehensive quality assurance audit. Your job is to systematically check every aspect of the platform — functionality, visual correctness, data integrity, routing, auth, and mobile responsiveness. Fix every issue you can. Report everything you find.

## How to Run This Skill

When invoked, work through every section below in order. Do not skip sections. Do not ask questions. Fix issues as you find them. Keep a running issue log.

---

## SECTION 1 — PRE-FLIGHT CHECK

Before auditing anything, establish baseline:

```bash
# 1. Confirm clean build
npx tsc --noEmit 2>&1 | head -30

# 2. Confirm no build errors
npm run build 2>&1 | tail -20

# 3. Check git status — nothing should be uncommitted
git status

# 4. Confirm which br
```

</details>
