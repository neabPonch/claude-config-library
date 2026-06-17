---
name: M5Fly-kanazawa__stampfly_ecosystem
source: https://github.com/M5Fly-kanazawa/stampfly_ecosystem/blob/5b2c41ba728e4b3d982bd76f82c9e15add1ef02e/CLAUDE.md
repo: M5Fly-kanazawa/stampfly_ecosystem
kind: claude-md
stars: 38
last_pushed: 2026-06-07T11:37:42Z
license: mit
score: 9
domains: [embedded-systems, robotics, engineering-workflow, ai-agents]
tags: [sub-agent-verification, simulation-first, bilingual-docs, diagram-quality]
curated: 2026-06-14
curated_by: config-scout
---

# M5Fly-kanazawa/stampfly_ecosystem — claude-md

**Why it's worth keeping:** The 'sub-agent + image conversion' loop for verifying LaTeX/PDF layouts is a top-tier agentic pattern; the mandate to back parameter changes with numerical simulation prevents AI hallucination in engineering tasks.

**Summary:** A high-precision engineering guide that defines strict workflows for control theory simulation, bilingual documentation standards, and automated visual verification.

**Source credibility:** High-quality educational/research repository for drone control engineering.

**Recency:** Very current, explicitly utilizing Claude Code's `/commit` skill and sub-agent patterns.

**Source:** [M5Fly-kanazawa/stampfly_ecosystem/CLAUDE.md](https://github.com/M5Fly-kanazawa/stampfly_ecosystem/blob/5b2c41ba728e4b3d982bd76f82c9e15add1ef02e/CLAUDE.md) · 38★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Session Rules

- **セッション開始時またはコンテキスト圧縮後に以下を読むこと:**
  - `PROJECT_PLAN.md`
  - `.claude/settings.local.json`
  - 前回のコミットログ（Next stepsから作業を再開）
- **応答は日本語で行うこと**
- **コードを変更したら必ずコミットすること** - 変更をローカルに残さず、適切な単位でコミットする
  - **必ず `/commit` スキルを使用する** - `docs/contributing/commit-guidelines.md` に基づいたコミットメッセージを自動作成
  - **Next steps セクションを必ず含める** - 次回セッション開始時のタスクを明記
  - 作業終了時、ファイル変更後、重要な節目で自動実行
- **sf CLI を積極的に使用すること** - ビルド、書き込み、診断などは `idf.py` を直接呼ぶのではなく `sf` コマンドを優先する
- **制御系パラメータの変更提案は必ず数値的シミュレーションで裏付けてから行うこと** - PIDゲイン、フィルタ定数、制御リミット等の変更を提案する際、実際のフライトログデータを使ったシミュレーションで効果を定量的に確認してから提示する。「Tiを短くすれば改善する」のような定性的な推測だけで提案しない。シミュレーションの結果、逆効果であれば提案しない

## Build Environment

### ESP-IDF
開発環境の初期化（`setup_env.sh` が ESP-IDF の `export.sh` を内部で呼ぶ）:
```bash
source setup_env.sh
```

ファームウェアのビルド:
```bash
cd firmware/vehicle  # or firmware/controller
idf.py build
idf.py flash monitor
```

### sf CLI（推奨）
sf CLI は ESP-IDF 環境に統合された開発ツール。`idf.py` を直接使う代わりにこちらを優先する：
```bash
source setup_env.sh  # 開発環境をアクティブ化（ESP-IDF + sf CLI）

sf doctor              # 環境診断（問題があればまずこれを実行）
sf build vehicle       # veh
```

</details>
