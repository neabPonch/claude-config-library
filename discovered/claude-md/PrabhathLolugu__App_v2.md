---
name: PrabhathLolugu__App_v2
source: https://github.com/PrabhathLolugu/App_v2/blob/01a289577c6f3ea8a46ad038c5ddcc51f49c4a4b/CLAUDE.md
repo: PrabhathLolugu/App_v2
kind: claude-md
stars: 0
last_pushed: 2026-04-11T08:34:59Z
license: unknown
score: 9
domains: [mobile-app, fullstack]
tags: [flutter, supabase, clean-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# PrabhathLolugu/App_v2 — claude-md

**Why it's worth keeping:** It provides explicit directory structures, specific coding patterns (like UseCase implementations), and critical code-generation workflows that prevent the AI from breaking the build.

**Summary:** A comprehensive guide for a Flutter/Supabase mobile app using Clean Architecture and DDD.

**Source credibility:** Personal repository with high-quality, implementation-specific documentation typical of professional Flutter development.

**Recency:** Current; utilizes modern package ecosystems like freezed, injectable, and go_router.

**Source:** [PrabhathLolugu/App_v2/CLAUDE.md](https://github.com/PrabhathLolugu/App_v2/blob/01a289577c6f3ea8a46ad038c5ddcc51f49c4a4b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MyItihas is a Flutter mobile app for cultural/historical stories from Indian scriptures. Features include social feeds, chat, AI story generation, and map features. Uses **Supabase** backend with offline-first local storage via **Hive**.

## Essential Commands

```bash
# Install dependencies
flutter pub get

# Code generation (CRITICAL - run after modifying @freezed, @injectable, routes, i18n, or .env)
dart run build_runner build --delete-conflicting-outputs

# Watch mode for code generation
dart run build_runner watch --delete-conflicting-outputs

# Generate translations only
dart run slang

# Run app
flutter run

# Analyze code
flutter analyze

# Run tests
flutter test
```

## Environment Variables (Envied)

Sensitive configuration is managed using the `envied` package with obfuscation enabled.

### Setup (Required for first-time setup)
1. Copy `.env.example` to `.env` in the project root
2. Fill in your Supabase credentials:
   ```
   SUPABASE_URL=https://your-project.supabase.co
   SUPABASE_ANON_KEY=your-anon-key
   ```
3. Run code generation
```

</details>
