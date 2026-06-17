---
name: sceneview__sceneview
source: https://github.com/sceneview/sceneview/blob/50cd5bd7d0f3952e2ee163e52e23d9b4ee63cfcb/CLAUDE.md
repo: sceneview/sceneview
kind: claude-md
stars: 1227
last_pushed: 2026-06-14T06:13:10Z
license: apache-2.0
score: 10
domains: [mobile-sdk, 3d-ar, qa-automation, devops]
tags: [ai-first, multiplatform, mobile-development, quality-assurance]
curated: 2026-06-15
curated_by: config-scout
---

# sceneview/sceneview — claude-md

**Why it's worth keeping:** It uses extremely specific command-line instructions instead of vague goals, defines a 'blocking vs advisory' hierarchy to handle flaky tests, and warns about highly specific technical landmines like the Filament ABI invariant.

**Summary:** Defines an AI-first development philosophy and provides rigorous, multi-platform verification protocols for a high-performance 3D/AR SDK.

**Source credibility:** Highly credible; 1.2k stars with very active, recent maintenance and sophisticated CI/QA workflows.

**Recency:** Current; utilizes modern tools including Maestro, Playwright, and Jetpack Compose ecosystem patterns.

**Source:** [sceneview/sceneview/CLAUDE.md](https://github.com/sceneview/sceneview/blob/50cd5bd7d0f3952e2ee163e52e23d9b4ee63cfcb/CLAUDE.md) · 1227★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SceneView — Claude Code guide

## Project purpose

SceneView is an **AI-first SDK**: its primary goal is to enable Claude (and other AI
assistants) to help developers build 3D and AR apps in Jetpack Compose. Every design
decision — API surface, documentation, samples, `llms.txt` — should be optimized so
that when a developer asks an AI "build me an AR app", the AI can produce correct,
complete, working code on the first try.

**Implication for contributors:** when adding or changing APIs, always ask "can an AI
read the docs and generate correct code for this?" If not, simplify the API or improve
the documentation until it can.

> **Start here.** Read [`.claude/STATE.md`](.claude/STATE.md) for *where we are* and
> [`.claude/workflows/README.md`](.claude/workflows/README.md) for *how we work* (the v2
> working methodology). This file holds stable project facts only — never session state.

## QUALITY RULES (MANDATORY — every session, every commit)

**ZERO TOLERANCE for bugs reaching the user.** Every change must be verified before push.

### Before EVERY push to main:
1. **Compile check**: `./gradlew :sceneview:compileReleaseKotlin :arsceneview:compileReleaseKotlin`
2. **Unit tests*
```

</details>
