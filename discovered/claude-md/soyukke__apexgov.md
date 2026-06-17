---
name: soyukke__apexgov
source: https://github.com/soyukke/apexgov/blob/461acd644475783684952daada9ebe1f09e84343/CLAUDE.md
repo: soyukke/apexgov
kind: claude-md
stars: 0
last_pushed: 2026-05-14T01:35:41Z
license: mit
score: 9
domains: [cli-tools, systems-programming, static-analysis]
tags: [zig, architecture-mapping, documentation]
curated: 2026-06-15
curated_by: config-scout
---

# soyukke/apexgov — claude-md

**Why it's worth keeping:** The table-driven breakdown of submodules is an elite pattern for context injection in complex projects; the explicit CLI command list facilitates immediate testing.

**Summary:** This config acts as a comprehensive architectural blueprint for a Zig-based tool, detailing subcommands and module responsibilities via structured tables.

**Source credibility:** Low star count, but appears to be a high-quality technical utility/tooling project.

**Recency:** Very current, pushed within the last month.

**Source:** [soyukke/apexgov/CLAUDE.md](https://github.com/soyukke/apexgov/blob/461acd644475783684952daada9ebe1f09e84343/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

apexgov は Salesforce Apex コード向けのオフライン静的チェッカー & デバッグログプロファイラー。CI/CD パイプラインでの利用を想定し、Governor 制限リスク（ループ内 SOQL/DML/Callout 等）の検出、デバッグログからの CPU/Heap 解析を提供する。

## ビルド & テスト

```bash
zig build                        # ビルド (zig-out/bin/apexgov)
zig build test                   # 全ユニットテスト実行
zig build run -- <subcommand>    # ビルド & 実行
```

主なサブコマンド:
- `check <path> [--format json|sarif|text]` — 静的解析
- `profile <path> [--format json|text]` — デバッグログプロファイル
- `interpret test <paths...>` — Zig ネイティブ Apex テスト実行
- `typegen <sfdx-project-root> [--out DIR]` — LWC 用 TypeScript 型定義生成
- `lsp` — Language Server Protocol サーバー起動（stdio）

Nix 開発環境: `nix develop` (Zig + ZLS)

## アーキテクチャ

### src/ — Zig コア (外部依存ゼロ)

- **main.zig** — CLI エントリポイント。サブコマンドルーティングと引数パース
- **model.zig** — 共通データ型 (`Severity`, `OutputFormat`, `Finding`, `ProfileResult`)
- **config.zig** — `apexgov.toml` の手書き TOML パーサー
- **report.zig** — text/json/sarif フォーマッター
- **profile.zig** — デバッグログパーサー。CPU/Heap 計測、マルチトランザクション分割、ベースライン比較

#### src/check/ — 静的解析エンジン（ファサード + 12 サブモジュール）

`check.zig` がファサードで、公開 API (`run`,
```

</details>
