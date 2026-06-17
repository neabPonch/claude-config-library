---
name: haruvv__dev-agents
source: https://github.com/haruvv/dev-agents/blob/f7e3c152a70b3bb4f222c6e1bc0f3f51dcb790ac/CLAUDE.md
repo: haruvv/dev-agents
kind: claude-md
stars: 0
last_pushed: 2026-04-07T17:44:38Z
license: unknown
score: 8
domains: [agents-ai, devops, automation]
tags: [multi-agent, orchestration, autonomous-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# haruvv/dev-agents — claude-md

**Why it's worth keeping:** It introduces a high-level pattern of segregating instructions into '.claude/agents/' and '.claude/skills/' to prevent context bloat. The mandatory 'planner' step provides a critical structural guardrail for autonomous task execution.

**Summary:** Orchestrates a multi-agent autonomous development pipeline by defining specialized sub-agents and modular skill sets stored in dedicated directories.

**Source credibility:** Low visibility (0 stars) from what appears to be a niche, specialized autonomous agent research project.

**Recency:** 

**Source:** [haruvv/dev-agents/CLAUDE.md](https://github.com/haruvv/dev-agents/blob/f7e3c152a70b3bb4f222c6e1bc0f3f51dcb790ac/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — dev-agents AI Worker 設定

このリポジトリ（`haruvv/dev-agents`）で動作する AI Worker 向けの設定ファイル。
Worker は GitHub Issue を受け取り、要件整理・設計・実装・修正を自律的に行う。

## パイプライン概要

```
GitHub Issue (labeled)
  → Worker ECS (Claude Code)
    → 要件定義 / 設計 / タスク分割 / 実装 / repair
      → PR 作成 → CI → レビュー
```

詳細は `AGENTS.md` を参照。

## エージェント

複雑なタスクには以下のサブエージェントを積極的に活用すること。

| エージェント | 用途 | 起動タイミング |
|---|---|---|
| `planner` | 実装計画の策定 | 実装着手前に必ず呼ぶ |
| `architect` | アーキテクチャ判断 | 設計の判断が必要なとき |
| `code-reviewer` | コードレビュー | コミット前に必ず呼ぶ |
| `security-reviewer` | セキュリティチェック | 認証・外部API・DB操作を含む実装時 |
| `code-explorer` | コードベース探索 | 既存コードを把握する必要があるとき |
| `doc-updater` | ドキュメント更新 | 実装変更後 |

エージェント定義: `.claude/agents/`

## スキル

以下のスキルが利用可能。必要に応じて参照すること。

| スキル | 内容 |
|---|---|
| `coding-standards` | コーディング規約・命名・品質基準 |
| `api-design` | REST API 設計パターン |
| `backend-patterns` | バックエンド設計パターン |
| `frontend-patterns` | フロントエンド設計パターン |
| `python-patterns` | Python ベストプラクティス |
| `python-testing` | Python テストパターン |
| `tdd-workflow` | TDD ワークフロー（Red-Green-Refactor） |
| `verification-loop` | 実装検証ループ |
| `plankton-code-quality` | コード品質チェック |
| `e2e-testing` | E2E テスト |

スキル定義: `.claude/skills/`

## 実装ルール

1. **実装前に必ず `planner` エージェントで
```

</details>
