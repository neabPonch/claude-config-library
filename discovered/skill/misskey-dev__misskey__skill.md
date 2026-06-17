---
name: misskey-dev__misskey__skill
source: https://github.com/misskey-dev/misskey/blob/f46450d8571b2c64a4732547884efc0cc60d81f6/.claude/skills/working-on-frontend/SKILL.md
repo: misskey-dev/misskey
kind: skill
stars: 11199
last_pushed: 2026-06-14T11:10:03Z
license: agpl-3.0
score: 9
domains: [web-frontend, vuejs, software-engineering-standards]
tags: [progressive-disclosure, workflow-orchestration, component-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# misskey-dev/misskey — skill

**Why it's worth keeping:** Demonstrates the 'progressive disclosure' pattern by linking to specific sub-skills to prevent context bloat. Also includes explicit mandates to re-invoke the skill at implementation time, preventing agents from skipping rules after high-level planning.

**Summary:** A high-precision entry point for frontend development that enforces strict project conventions, i18n rules, and component standards. It uses a hierarchical structure to manage complex technical requirements via progressive disclosure.

**Source credibility:** Extremely high; part of a major, highly-starred open-source project (Misskey) with active maintenance.

**Recency:** Current; reflects modern Vue 3/TypeScript standards and sophisticated AI agent orchestration techniques.

**Source:** [misskey-dev/misskey/.claude/skills/working-on-frontend/SKILL.md](https://github.com/misskey-dev/misskey/blob/f46450d8571b2c64a4732547884efc0cc60d81f6/.claude/skills/working-on-frontend/SKILL.md) · 11199★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: working-on-frontend
description: Use whenever editing or adding code under `packages/frontend/`, or editing `locales/ja-JP.yml` for frontend-facing UI text — including Vue 3 SFCs (`Mk*` components), i18n keys (`i18n.ts.<key>` / `i18n.tsx.<key>()`), SCSS Modules, theme/CSS variables, `os.*` UI helpers, and Storybook stories. Covers SPDX (HTML comment form), `<script setup lang="ts">` conventions, type-only defineProps, `ja-JP.yml`-only locale editing (other locale yml files are Crowdin-managed and must not be edited), and accessibility. Must be consulted before any frontend or UI-locale change to avoid CI failures, lost translations, and reviewer pushback. This is NOT waived by having already invoked brainstorming, writing-plans, or any other upstream skill — invoke this at implementation time regardless of what preceded it.
---

# working-on-frontend

`packages/frontend/` (Misskey Web クライアント) を編集するとき、最初に参照するスキル。Vue 3 SFC / SCSS Modules / i18n / `os.*` / Storybook / アクセシビリティの **手順** と **背景知識** をまとめている。

SKILL.md 本体は references への索引だけ。具体的な手順や規約は該当ファイルを Read すること (progressive disclosure)。

**他スキル実行後も免除されない。** `brainstorming` / `writing-plans` / その他アップストリームスキルを先に呼んでいても、`packa
```

</details>
