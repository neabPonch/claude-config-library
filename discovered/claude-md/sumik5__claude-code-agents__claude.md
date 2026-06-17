---
name: sumik5__claude-code-agents__claude
source: https://github.com/sumik5/claude-code-agents/blob/76151151688d77bcd28a4901074f69ff7ecb017a/start-agents/CLAUDE.md
repo: sumik5/claude-code-agents
kind: claude-md
stars: 0
last_pushed: 2025-07-17T05:17:16Z
license: mit
score: 8
domains: [cli-tools, agents-ai, systems-automation]
tags: [tmux, multi-agent, session-management, self-documenting]
curated: 2026-06-14
curated_by: config-scout
---

# sumik5/claude-code-agents — claude-md

**Why it's worth keeping:** It includes a crucial 'Document Maintenance' section that instructs the LLM to update CLAUDE.md itself when the project evolves. This prevents documentation rot in long-running projects.

**Summary:** Provides detailed operational commands for managing multi-agent tmux sessions and explains a complex tool architecture.

**Source credibility:** Low; personal repository with zero stars and no description.

**Recency:** 11 months old, but contains modern patterns for agentic orchestration.

**Source:** [sumik5/claude-code-agents/start-agents/CLAUDE.md](https://github.com/sumik5/claude-code-agents/blob/76151151688d77bcd28a4901074f69ff7ecb017a/start-agents/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 開発コマンド

### ビルドとテスト
```bash
# 依存関係の取得とビルド
make build

# テストの実行
make test

# リンターとフォーマットの実行
make lint
make fmt

# 単一テストの実行
go test -v ./internal/config -run TestLoadConfig
```

### インストールとクリーンアップ
```bash
# システムへのインストール
make install

# 成果物のクリーンアップ
make clean
```

### セッション管理
```bash
# セッション作成（統合監視画面）
./build/claude-code-agents ai-teams

# セッション作成（個別セッション）
./build/claude-code-agents ai-teams --layout individual

# 既存セッションのリセット
./build/claude-code-agents ai-teams --reset

# セッション一覧表示
./build/claude-code-agents --list

# セッション削除
./build/claude-code-agents --delete ai-teams

# 設定表示
./build/claude-code-agents --show-config
```

## アーキテクチャ概要

### 主要コンポーネント

1. **cmd**: コマンドライン引数の解析とサブコマンド処理
   - 起動オプションの管理（--debug, --verbose, --reset等）
   - セッション操作コマンド（--list, --delete等）
   - 設定表示コマンド（--show-config, --config等）

2. **config**: アプリケーション設定とリソース監視
   - JSON設定ファイルの読み込み/保存
   - デフォルト設定の管理（~/.claude/claude-code-agents/）
   - リソース監視（メモリ、CPU使用量チェック）

3. **launcher**: システム起動とtmuxセッション管理
   - 環境検証（Claude CLI、認証状態の確認）
   - 統合監視画面（6ペイン構成）と個別セッション方式
   - エージェント配置（PO/Manager/Dev1-4）

4.
```

</details>
