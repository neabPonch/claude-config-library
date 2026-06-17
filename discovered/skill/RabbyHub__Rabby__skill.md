---
name: RabbyHub__Rabby__skill
source: https://github.com/RabbyHub/Rabby/blob/c9ff0cc1a138b0deadc5ade5445a1b68ba43a8ba/skills/rabby-i18n-translation/SKILL.md
repo: RabbyHub/Rabby
kind: skill
stars: 1845
last_pushed: 2026-06-15T08:38:36Z
license: other
score: 9
domains: [web-frontend, i18n]
tags: [localization, json-manipulation, data-integrity]
curated: 2026-06-15
curated_by: config-scout
---

# RabbyHub/Rabby — skill

**Why it's worth keeping:** It demonstrates excellent 'Skip Rule' logic to handle metadata-driven exclusions and provides a rigorous validation checklist including placeholder parity and JSON structural integrity.

**Summary:** A highly specialized instruction set for synchronizing localization files by backfilling missing English keys into other locales.

**Source credibility:** High; Rabby is a major, well-maintained Ethereum wallet repository with high star count.

**Recency:** Current; reflects modern software localization workflows.

**Source:** [RabbyHub/Rabby/skills/rabby-i18n-translation/SKILL.md](https://github.com/RabbyHub/Rabby/blob/c9ff0cc1a138b0deadc5ade5445a1b68ba43a8ba/skills/rabby-i18n-translation/SKILL.md) · 1845★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rabby-i18n-translation
description: When updating `_raw/locales` translation files in the Rabby repository, backfill only non-skipped English leaf keys that are missing or empty in other locales, preserve placeholders, and respect `__skip_translation` markers.
metadata:
  short-description: Rabby i18n translation backfill rules
---

# Rabby I18n Translation

Use this playbook when editing locale JSON files under:

- `_raw/locales/*/messages.json`

When adding or removing a supported language, also update:

- `_raw/locales/index.json`

The browser extension manifest locale files under `_raw/_locales/*/messages.json` use Chrome `message`/`description` objects. Edit them only when the task explicitly targets extension manifest metadata, and preserve that object shape.

## Scope

Backfill only leaf string keys where English has a non-empty value and the target locale either:

- does not have the key
- has the key with an empty string value

Do not rewrite existing non-empty translations during a missing-key backfill.

## Skip Rules

Always evaluate `__skip_translation` before deciding what is missing.

1. `__skip_translation: true`

   The entire object is excluded from trans
```

</details>
