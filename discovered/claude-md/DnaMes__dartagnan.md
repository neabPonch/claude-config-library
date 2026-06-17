---
name: DnaMes__dartagnan
source: https://github.com/DnaMes/dartagnan/blob/f05d4d6dc47cb0efbe5bdaa8e38db70410d9aa4b/CLAUDE.md
repo: DnaMes/dartagnan
kind: claude-md
stars: 0
last_pushed: 2026-06-11T04:32:29Z
license: agpl-3.0
score: 9
domains: [mobile-app, flutter-dart]
tags: [architecture-constraints, rules-engine, offline-first]
curated: 2026-06-16
curated_by: config-scout
---

# DnaMes/dartagnan — claude-md

**Why it's worth keeping:** The 'Rules Engine' section is a masterclass in providing deterministic constraints to prevent an AI from introducing side effects into core logic. It also includes highly actionable command workflows for code generation and database migrations.

**Summary:** A high-density developer guide providing exhaustive context on project structure, tech stack, and strict architectural boundaries.

**Source credibility:** Low-star personal project, but documentation density suggests a high level of professional discipline.

**Recency:** Current; uses modern Flutter/Riverpod patterns.

**Source:** [DnaMes/dartagnan/CLAUDE.md](https://github.com/DnaMes/dartagnan/blob/f05d4d6dc47cb0efbe5bdaa8e38db70410d9aa4b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dartagnan — Developer Guide

## Was ist das?

Offline-first Flutter Darts-Scoring-App für Android + iOS. Eine Codebasis, keine Cloud, kein Backend. Spieler tragen Punkte per Pass-and-Play ein. Die App heißt **Dartagnan**.

## Versionierung-Policy

**Jedes geshippte Backlog-Item bumpt die Version um einen Patch.** Größere Themen-Bündel (mehrere Features im selben Release) können einen Minor-Bump bekommen. Major nur bei Breaking Changes (DB-Schema-Inkompatibilität).

Format: `MAJOR.MINOR.PATCH+BUILD`. BUILD ist eine monoton steigende Zahl (für Android `versionCode`).

**Pflicht-Schritte beim Shipping:**
1. `pubspec.yaml` — `version:` bumpen
2. `CHANGELOG.md` — Eintrag oben im richtigen Bereich (Added / Fixed / Changed / Removed)
3. `BACKLOG.md` — Item von `[ ]` auf `[x]` mit Versionsnummer
4. Atomic commit: ein Backlog-Item = ein Commit (Fixes können bündeln, Features lieber einzeln)
5. Bei jedem dritten/vierten Patch: APK rebuild + sideload

## Flutter ausführen

```bash
FLUTTER=/home/dnames/.local/share/mise/installs/flutter/3.41.9/bin/flutter
$FLUTTER pub get
$FLUTTER analyze          # muss 0 Fehler zeigen
$FLUTTER test             # alle Tests grün
$FLUTTER run              #
```

</details>
