---
name: K3vinb5__unyo-app__skill
source: https://github.com/K3vinb5/unyo-app/blob/0a44722edabedfa9c1d23804a8638516f8b42306/.agents/skills/unyo-routing-navigation/SKILL.md
repo: K3vinb5/unyo-app
kind: skill
stars: 638
last_pushed: 2026-06-12T15:01:53Z
license: bsd-3-clause
score: 8
domains: [mobile-app, flutter]
tags: [routing, navigation, autoroute, bloc]
curated: 2026-06-15
curated_by: config-scout
---

# K3vinb5/unyo-app — skill

**Why it's worth keeping:** It offers highly actionable, step-by-step workflows for adding new routes and demonstrates how to implement side-effect driven navigation from Cubits.

**Summary:** Provides a comprehensive guide to managing routing via AutoRoute, including nested structures and transition styles. It details a specific pattern for triggering navigation through an 'Effect' system to decouple business logic from BuildContext.

**Source credibility:** High; the source repository is active and well-starred (638 stars).

**Recency:** Current; updated within the last month.

**Source:** [K3vinb5/unyo-app/.agents/skills/unyo-routing-navigation/SKILL.md](https://github.com/K3vinb5/unyo-app/blob/0a44722edabedfa9c1d23804a8638516f8b42306/.agents/skills/unyo-routing-navigation/SKILL.md) · 638★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unyo-routing-navigation
description: How to add routes, configure navigation, and use AutoRoute in the Unyo Flutter app. Use this skill whenever adding new screens/routes, configuring nested tab navigation, defining route transitions, navigating between screens from cubits via effects, or debugging routing issues like "route not found" errors.
---

# Unyo Routing & Navigation

Unyo uses **AutoRoute** for type-safe declarative routing. Routes are defined in a single `AppRouter` class, and code generation creates the `.gr.dart` file with typed route pages. Navigation from cubits uses the Effect system rather than direct `BuildContext`.

## Architecture Overview

```
lib/core/router/
├── app_router.dart       # Route definitions (the source of truth)
└── app_router.gr.dart    # Generated file (DO NOT EDIT)
```

The router is instantiated once in `main.dart`:

```dart
final _appRouter = AppRouter();
```

And used in `MaterialApp.router()`:

```dart
MaterialApp.router(
  routerConfig: _appRouter.config(),
)
```

## Route Configuration

All routes are defined in `lib/core/router/app_router.dart` as a nested tree:

```dart
@AutoRouterConfig(replaceInRouteName: 'Screen|Page,Route
```

</details>
