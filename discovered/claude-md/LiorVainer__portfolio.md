---
name: LiorVainer__portfolio
source: https://github.com/LiorVainer/portfolio/blob/936e5ac9a2a04662558a2adb5b9b03b39782ab4b/CLAUDE.md
repo: LiorVainer/portfolio
kind: claude-md
stars: 0
last_pushed: 2026-01-19T12:20:05Z
license: unknown
score: 8
domains: [web-frontend, nextjs, typescript]
tags: [spec-driven, guardrails, build-validation]
curated: 2026-06-16
curated_by: config-scout
---

# LiorVainer/portfolio — claude-md

**Why it's worth keeping:** The mandatory 'run build after every change' workflow prevents error accumulation, and the use of an external specification file (@/openspec) provides high-level architectural guardrails for AI agents.

**Summary:** Implements a 'spec-driven' development pattern using a dedicated OpenSpec directory and enforces strict type/build validation.

**Source credibility:** Low (individual personal portfolio), but technical sophistication is evident.

**Recency:** Highly current; includes cutting-edge tech like Tailwind v4 and React 19.

**Source:** [LiorVainer/portfolio/CLAUDE.md](https://github.com/LiorVainer/portfolio/blob/936e5ac9a2a04662558a2adb5b9b03b39782ab4b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

<!-- OPENSPEC:START -->
## OpenSpec Instructions

These instructions are for AI assistants working in this project.

Always open `@/openspec/AGENTS.md` when the request:
- Mentions planning or proposals (words like proposal, spec, change, plan)
- Introduces new capabilities, breaking changes, architecture shifts, or big performance/security work
- Sounds ambiguous and you need the authoritative spec before coding

Use `@/openspec/AGENTS.md` to learn:
- How to create and apply change proposals
- Spec format and conventions
- Project structure and guidelines

Keep this managed block so 'openspec update' can refresh the instructions.

<!-- OPENSPEC:END -->

## Commands

```bash
pnpm dev          # Start development server at localhost:3000
pnpm build        # Production build
pnpm lint         # Run Biome linter (biome check)
pnpm format       # Format code with Biome (biome format --write)
pnpm tsc          # Type check (run after making changes)
```

## Architecture

This is a Next.js 16 portfolio site using the App Router with React 19.

**Key Technologies:**
- **Sty
```

</details>
