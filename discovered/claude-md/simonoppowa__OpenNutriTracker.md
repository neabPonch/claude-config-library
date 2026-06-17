---
name: simonoppowa__OpenNutriTracker
source: https://github.com/simonoppowa/OpenNutriTracker/blob/be18c117eafb0bbe8405bbc018f81329a432e40d/CLAUDE.md
repo: simonoppowa/OpenNutriTracker
kind: claude-md
stars: 1976
last_pushed: 2026-06-10T18:45:49Z
license: gpl-3.0
score: 9
domains: [mobile-development, flutter]
tags: [code-generation, accessibility, testing-automation, environment-config]
curated: 2026-06-15
curated_by: config-scout
---

# simonoppowa/OpenNutriTracker — claude-md

**Why it's worth keeping:** Uses highly effective structured tables to map file changes to specific generation tools and provides an exhaustive, rule-based system for accessibility identifiers used in UI testing.

**Summary:** Provides high-density operational instructions for a Flutter project, covering complex code-generation triggers and localization workflows.

**Source credibility:** Highly credible; the repository is popular (1900+ stars) and actively maintained.

**Recency:** Very current, utilizing modern toolsets like FVM and justfile.

**Source:** [simonoppowa/OpenNutriTracker/CLAUDE.md](https://github.com/simonoppowa/OpenNutriTracker/blob/be18c117eafb0bbe8405bbc018f81329a432e40d/CLAUDE.md) · 1976★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OpenNutriTracker is a Flutter mobile app (iOS/Android) for nutritional tracking. It uses Open Food Facts and USDA Food Data Central (via Supabase) as food databases, with all user data stored locally in an AES-encrypted Hive database.

Flutter version: **3.41.7** (managed via FVM; see `.fvmrc`)

## Commands

All common tasks are in the `justfile`:

```sh
just install       # flutter pub get
just build         # dart run build_runner build --delete-conflicting-outputs
just format        # dart format ./lib/core ./lib/features ./lib/l10n ./test
just test          # flutter test
just check_intl    # verify generated intl files are up to date (used in CI)
just ci            # full CI: install, format check, intl check, build, analyze, test
```

Run a single test file:

```sh
flutter test test/unit_test/tdee_calc_test.dart
```

Run static analysis:

```sh
flutter analyze
```

## Environment Setup

Copy `.env.example` to `.env` and fill in real values before running:

```sh
cp .env.example .env
```

The template carries placeholders that have no real-w
```

</details>
