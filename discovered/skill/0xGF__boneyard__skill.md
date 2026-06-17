---
name: 0xGF__boneyard__skill
source: https://github.com/0xGF/boneyard/blob/6629403ad0c21b75359be5ca5bce8fb5b136ca55/.claude/skills/boneyard/SKILL.md
repo: 0xGF/boneyard
kind: skill
stars: 5886
last_pushed: 2026-05-06T16:20:37Z
license: mit
score: 9
domains: [web-frontend, cli-tools, ui-frameworks]
tags: [skeleton-loading, documentation, component-library]
curated: 2026-06-15
curated_by: config-scout
---

# 0xGF/boneyard — skill

**Why it's worth keeping:** It includes critical low-level implementation details like bone resolution priority and internal array formats that a standard README might omit. This enables an agent to perform complex debugging and configuration tasks rather than just providing basic usage examples.

**Summary:** Provides deep technical documentation for the boneyard-js skeleton loading framework, covering architecture, CLI commands, and component props.

**Source credibility:** High; the source repository has significant social proof (5.8k stars) and recent activity.

**Recency:** Highly current; structured effectively for modern LLM tool-use and reasoning.

**Source:** [0xGF/boneyard/.claude/skills/boneyard/SKILL.md](https://github.com/0xGF/boneyard/blob/6629403ad0c21b75359be5ca5bce8fb5b136ca55/.claude/skills/boneyard/SKILL.md) · 5886★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: boneyard
description: Use boneyard-js to add, configure, debug, or rebuild skeleton screens. Triggers when working with Skeleton components, bones JSON, the boneyard CLI, fixtures, leafTags, snapshotConfig, skeleton loading states, or boneyard.config.json.
allowed-tools: Bash Read Edit Write Glob Grep Agent
---

# Boneyard Skeleton Skill

You are an expert on `boneyard-js`, a skeleton screen generator that snapshots real UI into positioned rectangle "bones". Use this knowledge to help with any boneyard-related task.

## Architecture

### Core files (in `packages/boneyard/`)
- `src/react.tsx` — `<Skeleton>` React component (also exports `configureBoneyard`, `registerBones`)
- `src/preact.tsx` — Native Preact integration (no compat needed)
- `src/Skeleton.svelte` — Svelte 5 component
- `src/Skeleton.vue` — Vue component
- `src/angular.ts` — Angular component
- `src/native.tsx` / `src/react-native.tsx` — React Native
- `src/extract.ts` — `snapshotBones()` DOM walker, `fromElement()` descriptor extractor
- `src/shared.ts` — bone registry, animation constants (`SHIMMER`, `PULSE`, `DEFAULTS`), `resolveResponsive`
- `src/types.ts` — `SnapshotConfig`, `Bone`, `CompactBone`, `Resp
```

</details>
