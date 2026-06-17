---
name: comeonzhj__Auto-Redbook-Skills
source: https://github.com/comeonzhj/Auto-Redbook-Skills/blob/6f06770f3662624760a0c885bca6230f40c8b7ad/SKILL.md
repo: comeonzhj/Auto-Redbook-Skills
kind: skill
stars: 1871
last_pushed: 2026-04-01T05:19:45Z
license: unknown
score: 9
domains: [content-creation, cli-tools, automation]
tags: [social-media, image-generation, workflow-orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# comeonzhj/Auto-Redbook-Skills — skill

**Why it's worth keeping:** It features a sophisticated multi-step pipeline that distinguishes between human-readable text and machine-renderable Markdown for visual assets. The highly specific command-line parameters for themes and pagination modes make the agent's tool usage precise and predictable.

**Summary:** A comprehensive skill that orchestrates content writing, image card rendering via HTML/CSS-to-PNG scripts, and social media publishing.

**Source credibility:** High credibility with 1871 stars and recent maintenance (2 months ago).

**Recency:** Highly current; utilizes modern CLI orchestration patterns suitable for Claude Code.

**Source:** [comeonzhj/Auto-Redbook-Skills/SKILL.md](https://github.com/comeonzhj/Auto-Redbook-Skills/blob/6f06770f3662624760a0c885bca6230f40c8b7ad/SKILL.md) · 1871★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: xhs-note-creator
description: 小红书笔记素材创作技能。当用户需要创建小红书笔记素材时使用这个技能。技能包含：根据用户的需求和提供的资料，撰写小红书笔记内容（标题+正文），生成图片卡片（封面+正文卡片），以及发布小红书笔记。支持 8 种精美排版主题和 4 种智能分页模式。
---

# 小红书笔记创作技能

根据用户提供的资料或需求，创作小红书笔记内容、生成精美图片卡片，并可选择发布到小红书。

> 详细参数文档见 `references/params.md`

---

## 工作流程

### 第一步：撰写小红书笔记内容

根据用户需求和资料，创作符合小红书风格的内容：

**标题**：不超过 20 字，吸引眼球，可用数字/疑问句/感叹号增强吸引力。

**正文**：段落清晰，点缀少量 Emoji（每段 1-2 个），短句短段，结尾附 5-10 个 SEO 标签。

---

### 第二步：生成渲染用 Markdown 文档

**注意：此 Markdown 专为图片渲染设计，禁止直接使用上一步的笔记正文。**

文档结构：

```markdown
---
emoji: "🚀"
title: "封面大标题（≤15字）"
subtitle: "封面副标题（≤15字）"
---

# 正文内容...

---

# 第二张卡片内容...（使用 --- 手动分隔时）
```

分页策略选择：
- 内容需精确切分 → 用 `---` 手动分隔，配合 `-m separator`
- 内容长短不稳定 → 生成普通 Markdown，使用 `-m auto-split`

---

### 第三步：渲染图片卡片

```bash
python scripts/render_xhs.py <markdown_file> [options]
```

**默认主题**：`sketch`（手绘素描风格）  
**默认分页**：`separator`（按 `---` 分隔）

常用示例：

```bash
# 默认（sketch 主题 + 手动分页）
python scripts/render_xhs.py content.md

# 自动分页（推荐内容长短不定时）
python scripts/render_xhs.py content.md -m auto-split

# 切换主题
python scripts/render_xhs.py content.md -t playful-geometric -m auto-split

# 固定尺寸自动缩放
python scripts/render_xhs.py content.md -m auto-fit
```

生成结果：`cover.png`（封面）+ `car
```

</details>
