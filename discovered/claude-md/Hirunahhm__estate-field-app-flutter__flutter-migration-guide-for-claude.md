---
name: Hirunahhm__estate-field-app-flutter__flutter-migration-guide-for-claude
source: https://github.com/Hirunahhm/estate-field-app-flutter/blob/7d79fa5fb2a9d13021adfe329a1b3568588afb0d/flutter_migration_guide_for_claude.md
repo: Hirunahhm/estate-field-app-flutter
kind: claude-md
stars: 0
last_pushed: 2026-03-20T05:03:38Z
license: unknown
score: 8
domains: [mobile-development, ui-migration]
tags: [flutter, tailwind, migration-logic, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# Hirunahhm/estate-field-app-flutter — claude-md

**Why it's worth keeping:** It provides explicit mappings between CSS layout concepts and Flutter widgets, while enforcing a strict 'Feature-First' folder structure through direct file path examples.

**Summary:** A specialized migration guide designed to transform HTML/Tailwind mockups into a structured, production-ready Flutter application.

**Source credibility:** Low; single developer repo with no stars or community validation.

**Recency:** Recent (3 months ago) and utilizes current industry standards like Riverpod and Material 3.

**Source:** [Hirunahhm/estate-field-app-flutter/flutter_migration_guide_for_claude.md](https://github.com/Hirunahhm/estate-field-app-flutter/blob/7d79fa5fb2a9d13021adfe329a1b3568588afb0d/flutter_migration_guide_for_claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# HTML to Flutter Migration Guide for Claude

This is the system prompt and instructional guide you should use when generating the Flutter code from the provided HTML mockups.

## Objective
Translate the Estate ERP Field App HTML mockups found in the `app in html` directory into production-ready Flutter Dart code, adhering strictly to the architecture defined in [coding_guide.md](file:///C:/Users/ASUS/.gemini/antigravity/brain/28f25ba6-a8cf-468e-b377-762c06a87d55/coding_guide.md).

---

## 🏗️ 1. Architecture Rules (Strict Enforcement)
- **Feature-First Structure**: Every UI screen MUST be placed in its respective feature folder.
  - [login.html](file:///e:/Porjects/Madukotawatte%20ERP/estate-field-app-flutter/app%20in%20html/login.html) ➡️ `lib/features/auth/presentation/screens/login_screen.dart`
  - [erp_home.html](file:///e:/Porjects/Madukotawatte%20ERP/estate-field-app-flutter/app%20in%20html/erp_home.html) ➡️ `lib/features/home/presentation/screens/home_screen.dart`
  - [tapper_selection_list.html](file:///e:/Porjects/Madukotawatte%20ERP/estate-field-app-flutter/app%20in%20html/tapper_selection_list.html) ➡️ `lib/features/hr/presentation/screens/tapper_attendance_screen.dart`
```

</details>
