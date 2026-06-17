---
name: beerock__my-workout-scheduler
source: https://github.com/beerock/my-workout-scheduler/blob/58e54245a1a5ae24ca1d73abd69549158a8381d1/CLAUDE.md
repo: beerock/my-workout-scheduler
kind: claude-md
stars: 2
last_pushed: 2026-05-13T21:27:13Z
license: unknown
score: 9
domains: [fullstack, automation, web-app]
tags: [gotchas, documentation-mapping, technical-guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# beerock/my-workout-scheduler — claude-md

**Why it's worth keeping:** The 'Critical Gotchas' section is a masterclass in teaching an AI project-specific edge cases, such as timezone nuances, database query patterns, and deployment quirks. The documentation lookup table effectively guides the agent through the codebase structure.

**Summary:** A high-signal configuration that provides a comprehensive document map and deep technical guardrails. It excels at preventing subtle logic errors by documenting 'Critical Gotchas'.

**Source credibility:** While the star count is low, the density of specific technical warnings suggests high-quality, practitioner-written documentation.

**Recency:** Very current; incorporates modern patterns for Next.js, Supabase, and Inngest.

**Source:** [beerock/my-workout-scheduler/CLAUDE.md](https://github.com/beerock/my-workout-scheduler/blob/58e54245a1a5ae24ca1d73abd69549158a8381d1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

**My Workout Scheduler** automates gym class reservations using Puppeteer to book classes the instant registration opens (e.g. 26 hours before class time).

**Tech Stack:** Next.js 16, TypeScript, Tailwind CSS, Supabase, Inngest, Puppeteer, Resend

**MVP Scope:** 5 users, 2-5 classes per user, 100% free tier services

**Current Version:** v2.37 - Booking History Dedup + Multi-Category Error Expansion (see PRD for full version history)

---

## Key Documentation

| Doc | Purpose | When to Use |
|-----|---------|-------------|
| [README.md](README.md) | Project overview, setup, tech stack | Onboarding, external-facing info |
| [PRD](docs/My%20Workout%20Scheduler%20PRD.md) | Full product spec, features, architecture | Understanding requirements, feature decisions |
| [BACKLOG.md](docs/BACKLOG.md) | Current priorities, pre-MVP tasks | What to work on next |
| [DESIGN_SYSTEM.md](docs/DESIGN_SYSTEM.md) | Colors, typography, spacing, patterns | Any UI/styling work |
| [COMPONENT_LIBRARY.md](docs/COMPONENT_LIBRARY.md) | Component APIs, usage examples | Building UI |
| [VOICE.md](docs/VOICE.md) | Voice registers, coach-voice tier mapping, section-name patte
```

</details>
