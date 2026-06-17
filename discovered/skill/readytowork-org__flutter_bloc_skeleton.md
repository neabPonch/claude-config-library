---
name: readytowork-org__flutter_bloc_skeleton
source: https://github.com/readytowork-org/flutter_bloc_skeleton/blob/324b40093be797719830877e1fba59536c79b32e/SKIll.md
repo: readytowork-org/flutter_bloc_skeleton
kind: skill
stars: 1
last_pushed: 2026-05-25T09:14:02Z
license: unknown
score: 9
domains: [mobile-development, flutter]
tags: [flutter, bloc, architecture, engineering-guide]
curated: 2026-06-14
curated_by: config-scout
---

# readytowork-org/flutter_bloc_skeleton — skill

**Why it's worth keeping:** The 'Generic checklist' provides a perfect execution plan for an agent; the vertical-slice folder rules strictly enforce dependency boundaries and prevent architectural drift.

**Summary:** A rigorous engineering guide for feature-driven Flutter architecture using BLoC and GetIt. It establishes strict protocols for adding new features to ensure routing, DI, and testing consistency.

**Source credibility:** Low social proof (1 star), but contains high-density technical instructions typical of professional enterprise standards.

**Recency:** Current; utilizes modern Flutter ecosystem patterns like go_router and strict linting.

**Source:** [readytowork-org/flutter_bloc_skeleton/SKIll.md](https://github.com/readytowork-org/flutter_bloc_skeleton/blob/324b40093be797719830877e1fba59536c79b32e/SKIll.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Flutter Bloc Skeleton — Engineering Guide

## Project overview

Flutter application using **BLoC** for state, **GetIt** for dependency injection, **Dio** for HTTP, and **go_router** for navigation. Business logic is grouped by **feature** under `lib/features/`. Shared UI and cross-cutting concerns live under `lib/core/` and `lib/shared/`. Localization is generated from ARB (`flutter gen-l10n`).

---

## Generic checklist — add a new page (any feature)

Use this order for **every** new screen so routing, DI, and tests stay consistent. Replace `<feature>` with the feature folder name (e.g. `auth`, `home`).

| Step | Action |
|------|--------|
| 1 | Place UI only under `lib/features/<feature>/presentation/`. Do not add feature pages under `lib/core/`. |
| 2 | Add **path** and **route name** in `presentation/routes/<feature>_route_paths.dart` (or extend the existing enum/constants for that feature). |
| 3 | Register a **`GoRoute`** in `presentation/routes/<feature>_routes.dart` pointing to your `const` page widget. |
| 4 | Compose routes in **`lib/core/routes/app_routes.dart`** (e.g. `...<Feature>Routes.routes`). If global redirects or `AppPage` need the new segment, update **`route_
```

</details>
