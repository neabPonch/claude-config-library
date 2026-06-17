---
name: ayutaz__piper-plus__skill
source: https://github.com/ayutaz/piper-plus/blob/7d3aa34e7acf5f8c91d6ad280aefbb369905db2a/.claude/skills/release-prep/SKILL.md
repo: ayutaz/piper-plus
kind: skill
stars: 174
last_pushed: 2026-06-14T16:41:38Z
license: mit
score: 9
domains: [cli-tools, devops, monorepo]
tags: [release-management, versioning, automation]
curated: 2026-06-15
curated_by: config-scout
---

# ayutaz/piper-plus — skill

**Why it's worth keeping:** Uses a highly reliable 'read-mostly' pattern that relies on tool-based data extraction (jq/curl) rather than LLM guesswork. The 3-way comparison logic (Local vs. Published vs. Canonical) is a perfect template for maintaining consistency in polyglot monorepos.

**Summary:** Automates high-stakes release preparation by auditing version consistency across multiple language manifests, remote registries, and a canonical source of truth.

**Source credibility:** High; source repo has strong star count and very recent activity.

**Recency:** Current; utilizes modern tool patterns like jq and shell-based manifest extraction well-suited for Claude Code.

**Source:** [ayutaz/piper-plus/.claude/skills/release-prep/SKILL.md](https://github.com/ayutaz/piper-plus/blob/7d3aa34e7acf5f8c91d6ad280aefbb369905db2a/.claude/skills/release-prep/SKILL.md) · 174★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-prep
description: 7 ランタイム manifest の version 一覧表示、CHANGELOG `[Unreleased]` → `[X.Y.Z]` 移行支援、公開 registry の最新公開 version 確認を 1 コマンドで実行する read-mostly skill。`docs/spec/release-versions.toml` を canonical source として参照。
argument-hint: "[runtime] [--target-version X.Y.Z]"
disable-model-invocation: true
allowed-tools: Bash(cat *) Bash(grep *) Bash(jq *) Bash(curl -s *) Bash(npm view *) Bash(git diff *) Bash(git log *) Bash(git status *) Bash(rg *) Read Edit Grep
---

# Release Preparation Helper

リリース作業の **forensic check** と **CHANGELOG 移行支援** を 1 つにまとめた skill。手動でやると忘れがちな以下 4 段階を 1 コマンドで通す:

1. 各 manifest の **現在の version** を一覧化 (7 runtime × 9 manifest)
2. `release-versions.toml` の `expected_prefix` との照合
3. CHANGELOG.md `[Unreleased]` の内容と、リリース時に必要な **昇格作業** の提案
4. 公開 registry (PyPI / crates.io / NuGet / npm / Maven Central) の **最新公開 version** 取得

実装は **read-mostly** — 変更提案は markdown diff 形式でユーザに提示し、 適用は明示確認後 (memory `feedback_merge_caution.md` に従う)。

## 引数

- `$ARGUMENTS` 空: 全 runtime を一覧
- `python` / `rust` / `csharp` / `npm` / `swift` / `kotlin`: 特定 runtime のみ
- `--target-version X.Y.Z`: 次回リリース予定 version (CHANGELOG 移行提案に使う)

## 現在の状態

- ブランチ: !`git rev-parse --abbrev-ref
```

</details>
