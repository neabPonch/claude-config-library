---
name: evanca__flutter-ai-rules__skill
source: https://github.com/evanca/flutter-ai-rules/blob/88ddad700c0cd33d40ab3781296295650e95ebde/skills/flutterfire-configure/SKILL.md
repo: evanca/flutter-ai-rules
kind: skill
stars: 571
last_pushed: 2026-06-08T08:42:47Z
license: mit
score: 9
domains: [mobile-development, cli-tools, cloud-services]
tags: [flutter, firebase, setup, flavors]
curated: 2026-06-15
curated_by: config-scout
---

# evanca/flutter-ai-rules — skill

**Why it's worth keeping:** Includes high-value patterns for multi-environment app flavors using namespace aliasing and provides exact terminal command sequences that reduce agent friction.

**Summary:** Provides a complete operational blueprint for setting up Firebase in Flutter via CLI tools and code initialization.

**Source credibility:** High; popular repository with recent activity and significant community validation.

**Recency:** Current; aligns with modern FlutterFire CLI workflows.

**Source:** [evanca/flutter-ai-rules/skills/flutterfire-configure/SKILL.md](https://github.com/evanca/flutter-ai-rules/blob/88ddad700c0cd33d40ab3781296295650e95ebde/skills/flutterfire-configure/SKILL.md) · 571★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: flutterfire-configure
description: "Sets up Firebase for Flutter apps using FlutterFire CLI. Use when adding Firebase to a Flutter project for the first time, running flutterfire configure after adding new platforms or services, initializing Firebase in main.dart, or configuring separate Firebase projects for multiple app flavors. Trigger terms: flutterfire configure, Firebase setup, Firebase initialization, firebase_core, firebase_options.dart, app flavors, multi-environment Firebase."
---

# FlutterFire Configure Skill

This skill defines how to correctly set up and configure Firebase for Flutter applications.

## When to Use

Use this skill when:

* Adding Firebase to a Flutter project for the first time.
* Running `flutterfire configure` after adding a new Firebase service or platform.
* Initializing Firebase in `main.dart`.
* Setting up separate Firebase projects for multiple app flavors.

---

## 1. Prerequisites

Install the required tools:

```bash
npm install -g firebase-tools
firebase login
dart pub global activate flutterfire_cli
```

**Minimum platform requirements:**
- Android: API level 19 (KitKat) or higher
- Apple: iOS 11 or higher

---

## 2. Setup and Co
```

</details>
