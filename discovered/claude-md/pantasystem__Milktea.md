---
name: pantasystem__Milktea
source: https://github.com/pantasystem/Milktea/blob/c3ebf4aabb949df43c8758499db19ef8e155e31d/CLAUDE.md
repo: pantasystem/Milktea
kind: claude-md
stars: 269
last_pushed: 2026-04-12T11:49:06Z
license: gpl-3.0
score: 9
domains: [mobile-android, devops, refactoring]
tags: [roadmap, checklist, migration-plan, android]
curated: 2026-06-16
curated_by: config-scout
---

# pantasystem/Milktea — claude-md

**Why it's worth keeping:** Provides exact file paths for every task, includes critical technical workarounds (like the ViewPager2 inset issue), and uses a checklist format that allows an agent to track state across long refactoring sessions.

**Summary:** A highly granular, multi-phase migration roadmap for upgrading an Android project to modern SDK and Material 3 standards.

**Source credibility:** High; comes from a popular open-source Android client with recent activity.

**Recency:** Extremely current, addressing modern Android 15/SDK 35 requirements.

**Source:** [pantasystem/Milktea/CLAUDE.md](https://github.com/pantasystem/Milktea/blob/c3ebf4aabb949df43c8758499db19ef8e155e31d/CLAUDE.md) · 269★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Milktea Android SDK 対応チェックリスト

このファイルはAndroid最新SDK対応の進捗管理用です。
作業完了したタスクは `- [ ]` を `- [x]` に変えてください。

---

## Phase 1: M3 テーマ基盤の構築

**全 Compose 作業の前提条件。最初に完了させる。**

### 1-1. XML テーマを Material3 に移行
- [x] `app/src/main/res/values-v23/themes.xml` — `Theme.MaterialComponents` → `Theme.Material3`、システムバー色属性を削除
- [x] `app/src/main/res/values-v27/themes.xml` — 同上
- [x] `modules/common_resource/src/main/res/values/themes.xml` — 同上（Dark/Black/Bread/ElephantDark テーマ）
- [x] `app/src/main/res/values-v21/styles.xml` — 古いスタイル整理
- [x] `modules/common_resource/src/main/res/values/styles.xml` — Widget.MaterialComponents.* → Widget.Material3.* に更新

### 1-2. Compose M3 テーマラッパーの作成
現在 `MdcTheme`（Material2 ブリッジ）を使用中 → M3 の `MaterialTheme` に置き換える。
- [x] `modules/common_compose/MilkteaTheme.kt` に M3 用 `ColorScheme` を 5テーマ分定義
  - White / Dark / Black / Bread / ElephantDark
  - `Theme.toColorScheme()` 拡張関数で ThemeUtil.kt の Theme enum と同期
- [x] `MdcTheme { }` → `MaterialTheme(colorScheme = ...) { }` に置き換え
- [x] `libs.versions.toml` に `compose-material3 = "1.3.1"` を追加
- [x] `common_compose/build.gradle` で material2 → material3 に差し替え、MdcTheme アダプター削除
- [x] ビルド確認（Phase 2 の import 置き換え前なのでコンパイルエラーが大量に出る想定）

---
```

</details>
