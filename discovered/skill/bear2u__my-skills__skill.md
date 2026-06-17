---
name: bear2u__my-skills__skill
source: https://github.com/bear2u/my-skills/blob/1be5394eca8fa177d4471348c0affcbaa7f55a8c/skills/flutter-init/SKILL.md
repo: bear2u/my-skills
kind: skill
stars: 874
last_pushed: 2026-02-08T04:10:50Z
license: unknown
score: 9
domains: [mobile-development, flutter]
tags: [scaffolding, clean-architecture, riverpod, automation]
curated: 2026-06-16
curated_by: config-scout
---

# bear2u/my-skills — skill

**Why it's worth keeping:** The skill includes a sophisticated self-healing loop that uses 'flutter analyze' to proactively fix common code-generation errors (like Freezed/Riverpod compatibility). It also manages complex environmental configuration like Android Kotlin DSL desugaring.

**Summary:** Automates full-stack Flutter project scaffolding using Clean Architecture, Riverpod 3.0, and Drift.

**Source credibility:** High; 874 stars and highly specialized, deep domain knowledge suggest a mature toolset.

**Recency:** Very current; explicitly targets Riverpod 3.0 and modern Flutter/Kotlin DSL standards.

**Source:** [bear2u/my-skills/skills/flutter-init/SKILL.md](https://github.com/bear2u/my-skills/blob/1be5394eca8fa177d4471348c0affcbaa7f55a8c/skills/flutter-init/SKILL.md) · 874★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: flutter-init
description: Use when user wants to create a new Flutter project (Todo/Habit/Note/Expense/Custom domain) with Clean Architecture, Riverpod 3.0, Drift, and modern Flutter stack
---

# Flutter Init Skill

도메인 기반 Flutter 프로젝트를 생성하고 현대적인 아키텍처로 자동 설정합니다.
Todo, Habit, Note, Expense 또는 Custom 도메인을 선택하여 Clean Architecture 기반의 완전한 CRUD 앱을 즉시 생성할 수 있습니다.

## Quick Start

스킬 실행 시 다음 정보를 입력받습니다:
- 폴더명 (예: my_habit_app)
- 프로젝트명/패키지명 (예: habit_app)
- 도메인 선택 (Todo/Habit/Note/Expense/Custom)
- 스택 프리셋 (Minimal/Essential/Full Stack/Custom)

그 후 자동으로 다음 단계가 실행됩니다:

```bash
# 1. 프로젝트 생성 (Android/Kotlin, iOS/Swift)
flutter create --platforms android,ios --android-language kotlin --org com.example [폴더명]

# 2. 패키지 설치
flutter pub get

# 3. 도메인별 Clean Architecture 코드 자동 생성
# - domain/entities/[domain].dart (Freezed 엔티티)
# - data/datasources/local/app_database.dart (Drift 테이블)
# - data/repositories/[domain]_repository_impl.dart (Repository 구현)
# - presentation/providers/[domain]_providers.dart (Riverpod 3.0)
# - presentation/screens/* (List/Detail/Form 화면)

# 4. 코드 생성 (Freezed, Drift, JSON Serializable)
dart run build_runner build --delete-conflicting-outputs

# 5. 코드 검증 및 오류 자동 수정 (필
```

</details>
