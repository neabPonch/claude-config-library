---
name: hiboma__hiboma
source: https://github.com/hiboma/hiboma/blob/258126bd712649504c2904f2594befd1f8bd7cfc/CLAUDE.md
repo: hiboma/hiboma
kind: claude-md
stars: 241
last_pushed: 2026-03-31T09:10:56Z
license: unknown
score: 7
domains: [security, systems-programming]
tags: [security-guardrails, data-privacy, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# hiboma/hiboma — claude-md

**Why it's worth keeping:** Demonstrates how to integrate custom security workflows by linking the main guide to specific `.claude/rules`, skills, and shell scripts.

**Summary:** Provides context for a technical Linux kernel knowledge base and establishes a rigorous sensitive-data scanning protocol.

**Source credibility:** High; authored by a Senior Principal Engineer with specialized system programming expertise.

**Recency:** Current; utilizes modern Claude Code features like .claude/rules and skills.

**Source:** [hiboma/hiboma/CLAUDE.md](https://github.com/hiboma/hiboma/blob/258126bd712649504c2904f2594befd1f8bd7cfc/CLAUDE.md) · 241★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## リポジトリの概要

Linux カーネル、システムプログラミング、インフラ技術に関する技術ノート・知識ベースです。ビルド対象のコードプロジェクトではなく、マークダウン文書の集合体です。

著者は GMO ペパボの Senior Principal Engineer で、トラブルシューティング、カーネルソースコードリーディング、CVE の PoC 検証、セキュリティ対策などを専門としています。

## 構造

- `kernel/` — Linux カーネル関連（サブディレクトリ: mm, net, fs, proc, block, ftrace, kvm, perf, sys）
- `tcp/` — TCP/IP スタックの詳細な技術ノート
- `auditd/` — Linux audit サブシステムの調査
- `books/` — 技術書の読書・学習記録
- `mysql/`, `httpd/`, `ruby/`, `jruby/` — ミドルウェア関連の調査
- `Linuxカーネル解読室/`, `CodeReading/`, `Linux_Kernel_Architecture/` — ソースコードリーディング記録
- `slides/` — 発表スライドの原稿
- `security/` — セキュリティ関連の調査
- ルート直下の `.md` ファイル — 個別のトピックごとの技術ノート

## 文書の特徴

- 日本語で記述されています
- カーネルソースコードの引用と解説が多く含まれます
- 実験手順と観察結果がセットで記録されています
- CVE の PoC 検証やバグレポートの記録も含まれます

## 秘匿情報スキャン

コマンド実行の履歴や出力をマークダウンに記録する際、秘匿情報や個人を特定できるディレクトリパスの漏洩を防止する仕組みがあります。

### 構成

| ファイル | 役割 |
|---|---|
| `scripts/scan-sensitive-data.sh` | 共通スキャンスクリプト。差分・ファイルから秘匿情報を検出します |
| `.claude/rules/sensitive-data-check.md` | Claude Code のルール。commit 前のスキャン実行を指示します |
| `.claude/skills/sensitive-data-guard.md` | Claude Code のスキル。マスク対象パターンとマスク手順を定義します |
| `.gi
```

</details>
