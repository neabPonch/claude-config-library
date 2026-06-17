---
name: athola__claude-night-market__skill
source: https://github.com/athola/claude-night-market/blob/cfe362f413c590983a7332364d718e08807838a5/plugins/scry/skills/media-composition/SKILL.md
repo: athola/claude-night-market
kind: skill
stars: 309
last_pushed: 2026-06-15T23:55:23Z
license: mit
score: 8
domains: [media-generation, cli-tools, automation]
tags: [ffmpeg, manifest-driven, orchestration]
curated: 2026-06-16
curated_by: config-scout
---

# athola/claude-night-market — skill

**Why it's worth keeping:** The skill uses a highly transferable 'Manifest-Driven' pattern where the agent reads configuration rather than following loose instructions; it also includes essential validation/verification steps to prevent execution loops.

**Summary:** Orchestrates FFmpeg to combine media assets into structured layouts (vertical, grid, etc.) using a declarative YAML manifest.

**Source credibility:** Strong; 309 stars and recently updated, indicating a high-quality, community-vetted repository.

**Recency:** Current; reflects modern agentic orchestration patterns suitable for Claude Code.

**Source:** [athola/claude-night-market/plugins/scry/skills/media-composition/SKILL.md](https://github.com/athola/claude-night-market/blob/cfe362f413c590983a7332364d718e08807838a5/plugins/scry/skills/media-composition/SKILL.md) · 309★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: media-composition
description: Combines GIFs and videos into composite tutorials with vertical or grid layouts via ffmpeg. Use when assembling multi-part media into a single output.
alwaysApply: false
category: media-generation
tags:
- composition
- ffmpeg
- media
- combine
- stitch
- tutorial
tools: []
complexity: medium
model_hint: standard
estimated_tokens: 450
progressive_loading: false
dependencies:
- scry:gif-generation
---
## Table of Contents

- [Overview](#overview)
- [Required TodoWrite Items](#required-todowrite-items)
- [Manifest Format](#manifest-format)
- [Manifest Schema](#manifest-schema)
- [Step-by-Step Process](#step-by-step-process)
- [1. Parse Manifest File](#1-parse-manifest-file)
- [2. Validate Component Outputs](#2-validate-component-outputs)
- [3. Execute FFmpeg Composition](#3-execute-ffmpeg-composition)
- [4. Verify Combined Output](#4-verify-combined-output)
- [FFmpeg Composition Commands](#ffmpeg-composition-commands)
- [Vertical Stacking](#vertical-stacking)
- [Horizontal Stacking](#horizontal-stacking)
- [Sequential Concatenation](#sequential-concatenation)
- [Grid Layout (2x2)](#grid-layout-(2x2))
- [With Background Color](#with-background-c
```

</details>
