---
name: hirokisakabe__pom__skill
source: https://github.com/hirokisakabe/pom/blob/286f7be8a01f8fb6e2bebc1c75bcf0816b96e9b3/skills/pom-slide/SKILL.md
repo: hirokisakabe/pom
kind: skill
stars: 7
last_pushed: 2026-06-15T00:17:21Z
license: mit
score: 9
domains: [design-systems, cli-tools, content-generation]
tags: [presentation, xml, design-system, automation]
curated: 2026-06-15
curated_by: config-scout
---

# hirokisakabe/pom — skill

**Why it's worth keeping:** It encodes specific mathematical constraints—such as an 8px spacing system, a 5-tier typography scale, and distinct slide archetypes—to prevent generic 'AI-looking' outputs. This technique teaches the agent how to act like a professional graphic designer rather than just a text writer.

**Summary:** Generates professional presentation slides from natural language by applying a strict design system to a custom XML format. It manages branding-aware themes, color roles, and structural archetypes for visual consistency.

**Source credibility:** Highly specialized tool with high engineering density despite low star count.

**Recency:** Current; maintained within the last month.

**Source:** [hirokisakabe/pom/skills/pom-slide/SKILL.md](https://github.com/hirokisakabe/pom/blob/286f7be8a01f8fb6e2bebc1c75bcf0816b96e9b3/skills/pom-slide/SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pom-slide
description: Generate pom presentation slides from natural language. Applies design principles (color palette, typography scale, spacing), honors a pom-theme.json brand theme when present, creates a pom XML file, performs a rendered self-review loop, and optionally launches a live preview with pom-cli.
license: MIT
allowed-tools: Write,Edit,Read,Bash
metadata:
  version: "1.3.1"
---

自然言語の指示から pom XML スライドを生成し、ファイルに保存する。デザイン原則（配色・タイポグラフィ・余白・アーキタイプ）に基づいて初版の質を高め、`/pom-theme` skill が生成したテーマファイル（`pom-theme.json`）があればブランド配色・フォントを適用する。レンダリング結果を自分で見て修正するセルフレビューを行ったうえで、pom-cli がインストール済みの場合はプレビューサーバーを起動する。

## 手順

### 1. 入力の解釈

ユーザーの指示からスライドの内容・枚数・テーマを把握する。

明示されていない場合のデフォルト:

- 枚数: 指示の内容量に適した枚数（3〜8 枚程度）
- ファイル名: `slides.pom.xml`

### 2. デザイン方針の決定

XML を書き始める前に、デッキ全体のデザイントークン（配色・タイポグラフィ・余白）を決める。場当たり的に色やサイズを選ばず、ここで決めた値だけを使ってデッキ全体を組む。

#### テーマファイルの確認

最初にカレントディレクトリ（またはユーザーが指定したディレクトリ）に `pom-theme.json` があるか確認する。あれば `Read` ツールで読み込み、以下のとおりデザイントークンとして採用する。`pom-theme.json` は `/pom-theme` skill が生成するテーマファイルで、ブランドに合わせた配色・フォントが定義されている。

- **トーン**: `tone` フィールドの値を採用する（下記「トーン」の選択をスキップ）
- **配色パレット**: `colors` の `base` / `surface` / `ink` / `muted` / `accent` を 5 ロールにそのまま使う（下記プリセットか
```

</details>
