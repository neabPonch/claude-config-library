---
name: classmethod__tsumiki__skill
source: https://github.com/classmethod/tsumiki/blob/9a0a2348ebf1cb83b7cf91adfe2ffff28be02525/skills/dev-webtest/SKILL.md
repo: classmethod/tsumiki
kind: skill
stars: 966
last_pushed: 2026-05-27T07:33:08Z
license: mit
score: 9
domains: [web-testing, automation, qa]
tags: [playwright, e2e, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# classmethod/tsumiki — skill

**Why it's worth keeping:** It features advanced agentic patterns like environmental knowledge persistence (learning from past failures) and a multi-layered concurrency model for parallelizing test groups.

**Summary:** A sophisticated Playwright orchestration skill that automates E2E, visual, and accessibility testing through structured execution plans.

**Source credibility:** Highly credible with nearly 1k stars on the source repository.

**Recency:** Very current, incorporating Playwright MCP workflows and modern Docker orchestration logic.

**Source:** [classmethod/tsumiki/skills/dev-webtest/SKILL.md](https://github.com/classmethod/tsumiki/blob/9a0a2348ebf1cb83b7cf91adfe2ffff28be02525/skills/dev-webtest/SKILL.md) · 966★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dev-webtest
description: This skill should be used when the user asks to "dev-webtest", "Webテスト", "画面の動作確認", "E2Eテスト", "web test", "visual check", "モンキーテスト", "アクセシビリティチェック", "レスポンシブテスト", "フォームテスト". Playwright CLIを使ってWebアプリの動作確認・視覚テスト・アクセシビリティ・レスポンシブ・フォームバリデーションを実行し、問題を検出・記録する。
argument-hint: '<plan-name> [--parallel N] | monkey <url> | check <url> | retest'
---

# Dev Webtest

Playwright CLI (`@playwright/cli`) を使ったWebアプリケーションの動作確認・視覚テスト・記録スキル。計画テスト、モンキーテスト、視覚チェック、アクセシビリティ、レスポンシブ、フォームバリデーションの6種類のテストを実行し、検出した問題をエラーディレクトリに記録する。修正は dev-debug 等の別スキルに委譲する。

## 前提知識

### dev-*スキルフロー内の位置

```
dev-context → dev-plan → dev-impl → dev-verify
                                         ↓
                                    [dev-webtest]
                                         ↓
                                    dev-debug (問題修正)
```

dev-verify でユニットテスト/ビルド/Lintが通った後にWeb画面の動作確認として使用する。単独での使用も可能。

### 実行モード

| モード | 引数 | 用途 |
|-------|------|------|
| 計画テスト | `<plan-name> [--parallel N]` | Markdownテスト計画に沿って自動テスト |
| モンキーテスト | `monkey <url>` | ランダム操作でエラー・崩れを検出 |
| クイックチェック | `check <url>` | 単一ページの視覚・アクセシビリティ確認 |
| プラン選択 | (引数なし) | 利用可能なプラン一覧から選択して実行 |
| 再テスト | `retest` | 未解決エラーの再現手順を再実
```

</details>
