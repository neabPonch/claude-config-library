---
name: hitosea__happy-next
source: https://github.com/hitosea/happy-next/blob/b163c3f618896afeb99a2425a6cba3aa97e7068d/CLAUDE.md
repo: hitosea/happy-next
kind: claude-md
stars: 35
last_pushed: 2026-06-09T23:25:21Z
license: mit
score: 7
domains: [fullstack-web, monorepo, ai-agents]
tags: [monorepo, build-workflows, interaction-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# hitosea/happy-next — claude-md

**Why it's worth keeping:** The 'happy-wire' build instruction is crucial—it tells the AI that changes won't propagate until a rebuild occurs, preventing stale-code debugging loops. The interaction rule to 'always suggest options' also optimizes agent efficiency.

**Summary:** Provides high-level context for a monorepo and specific technical workflows for package dependencies.

**Source credibility:** Active project with moderate social proof (35 stars).

**Recency:** Current; uses modern technologies like Expo, Fastify, and Vitest.

**Source:** [hitosea/happy-next/CLAUDE.md](https://github.com/hitosea/happy-next/blob/b163c3f618896afeb99a2425a6cba3aa97e7068d/CLAUDE.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Interaction Rules

- **Always suggest options when asking questions** — when clarifying requirements, provide concrete recommendations or choices to help the user decide quickly, rather than open-ended questions

## Language Preference

- Respond in Simplified Chinese unless the user explicitly requests another language

## Repository Overview

Yarn 1.x monorepo (`yarn@1.22.22`).

| Package | Purpose |
|---------|---------|
| **happy-app** | Expo/React Native mobile + web client |
| **happy-cli** | CLI wrapper for Claude Code, Codex, Gemini |
| **happy-server** | Fastify backend (API + Socket.IO) |
| **happy-voice** | LiveKit-based voice gateway |
| **happy-wire** | Shared Zod schemas and wire types |

## Type Checking (run after all changes)

Run `yarn typecheck` in the package you modified. In happy-server the command is `yarn build` (which is `tsc --noEmit`, not a real build step).

## happy-wire (run after every change)

After modifying the **happy-wire** package, always run `yarn build` in it — consumers depend on its compiled `dist` output, so changes won't take effect until rebuilt.

## Running a Single Test (Vitest)

```bash
npx vitest run path/to/file.test.ts
```
```

</details>
