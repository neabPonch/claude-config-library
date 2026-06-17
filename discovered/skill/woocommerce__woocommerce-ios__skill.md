---
name: woocommerce__woocommerce-ios__skill
source: https://github.com/woocommerce/woocommerce-ios/blob/741963aecc17d0afce8deb649613d1d9d590b67e/.claude/skills/review/SKILL.md
repo: woocommerce/woocommerce-ios
kind: skill
stars: 359
last_pushed: 2026-06-15T01:08:25Z
license: gpl-2.0
score: 9
domains: [ios-development, mobile-app, qa-automation]
tags: [swift, code-review, standardization, git]
curated: 2026-06-15
curated_by: config-scout
---

# woocommerce/woocommerce-ios — skill

**Why it's worth keeping:** It utilizes a modular design by referencing specialized rule files rather than bloating the skill file, and provides precise shell commands to extract change context.

**Summary:** Automates code reviews by comparing git diffs against a highly structured set of architectural, stylistic, and localization standards.

**Source credibility:** High-quality source from a major enterprise open-source project (WooCommerce).

**Recency:** Very current; uses standard git workflows and integrates seamlessly with agentic toolsets.

**Source:** [woocommerce/woocommerce-ios/.claude/skills/review/SKILL.md](https://github.com/woocommerce/woocommerce-ios/blob/741963aecc17d0afce8deb649613d1d9d590b67e/.claude/skills/review/SKILL.md) · 359★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: review
description: Review code changes against WooCommerce iOS standards
user-invocable: true
allowed-tools: "Bash, Read, Grep, Glob"
---

Review the current changes for compliance with WooCommerce iOS conventions.

1. Get the changes to review:
```bash
git diff trunk...HEAD
```
If no diff against trunk, fall back to staged changes: `git diff --cached`

2. Check each modified file against these criteria:

**Architecture** (see `.claude/rules/architecture.md`):
- UI code does not import Networking or Storage directly
- New actions follow the Yosemite dispatch pattern
- Dependencies injected via constructor with protocol types
- Coordinators for navigation, ViewModels for state

**Swift Style** (see `.claude/rules/swift-style.md`):
- No force unwraps or force casts
- Error handling uses do-catch, not try?
- Line length under 163 characters
- No parentheses around conditionals

**Localization** (see `.claude/rules/localization.md`):
- NSLocalizedString uses reverse-DNS keys with value: and comment:
- No LocalizedStringKey
- No string interpolation in localized strings
- Positional placeholders (%1$@)
- Strings grouped in enum Localization { }

**Analytics** (see `.claude/ru
```

</details>
