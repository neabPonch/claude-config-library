---
name: RSSNext__Folo__skill
source: https://github.com/RSSNext/Folo/blob/c98f572cf89a659c319bca598ffddf0654a7453a/.agents/skills/mobile-release/SKILL.md
repo: RSSNext/Folo
kind: skill
stars: 38480
last_pushed: 2026-06-05T11:44:07Z
license: agpl-3.0
score: 9
domains: [mobile-dev, devops]
tags: [mobile, release-automation, git, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# RSSNext/Folo — skill

**Why it's worth keeping:** Uses highly specific path-based decision logic and incorporates an ingenious 'runtime check' via curl to prevent deployment mismatches. The pattern of gathering state, presenting a draft, and requiring explicit user confirmation is an elite template for high-stakes procedures.

**Summary:** Automates a complex mobile deployment workflow by deciding between native app store releases and OTA (Over-The-Air) updates based on changed file paths. It handles changelog generation, version synchronization with external stores, and PR creation.

**Source credibility:** High; sourced from a widely recognized, actively maintained mobile application repository (38k+ stars).

**Recency:** Current; demonstrates advanced orchestration patterns ideal for Claude Code's tool usage capabilities.

**Source:** [RSSNext/Folo/.agents/skills/mobile-release/SKILL.md](https://github.com/RSSNext/Folo/blob/c98f572cf89a659c319bca598ffddf0654a7453a/.agents/skills/mobile-release/SKILL.md) · 38480★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mobile-release
description: Use when preparing a mobile release from the dev branch and deciding whether changes should ship through the app stores or through the OTA pipeline before creating the release PR to mobile-main.
disable-model-invocation: true
allowed-tools: Bash, Read, Write, Edit, Glob, Grep
---

# Mobile Release

Perform a mobile release from `dev`, with an explicit release-mode decision before the bump.

The skill must recommend one of these modes, explain why, ask the user to confirm, and then write `apps/mobile/release-plan.json` before running the bump:

- `store`: normal App Store / Google Play release
- `ota`: OTA-only publish, no store builds

Do not recommend or write any other mode. The current implementation only supports `store` and `ota`.

The CI release flow is file-driven:

- `apps/mobile/release-plan.json` is the editable plan on `dev`
- `pnpm bump` runs `apps/mobile/scripts/apply-release-config.ts`
- that script writes `apps/mobile/release.json` for the new version and resets the plan back to a safe default
- GitHub Actions reads `apps/mobile/release.json` after merge to decide which pipelines to trigger

## Pre-flight checks

1. Confirm the c
```

</details>
