---
name: op7418__Document-illustrator-skill
source: https://github.com/op7418/Document-illustrator-skill/blob/8344815d407cc25cc04c327557f36ed839f0aaef/SKILL.md
repo: op7418/Document-illustrator-skill
kind: skill
stars: 547
last_pushed: 2026-01-21T09:47:26Z
license: mit
score: 9
domains: [agents-ai, content-creation, cli-tools]
tags: [illustration, image-generation, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# op7418/Document-illustrator-skill — skill

**Why it's worth keeping:** The structured 'Ask -> Summarize -> Confirm' loop is a perfect template for complex agent tasks; the highly specific style/ratio definitions demonstrate how to encode visual consistency into a skill.

**Summary:** An automated pipeline that analyzes documents to generate a series of themed illustrations in specific aesthetic styles. It uses an interactive multi-step workflow to ensure user intent matches the AI's summarization before execution.

**Source credibility:** Strong popularity with 547 stars and professional-grade documentation.

**Recency:** Current, updated within the last 5 months.

**Source:** [op7418/Document-illustrator-skill/SKILL.md](https://github.com/op7418/Document-illustrator-skill/blob/8344815d407cc25cc04c327557f36ed839f0aaef/SKILL.md) · 547★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: document-illustrator
description: >
  基于文档内容自动生成配图。AI 智能分析文档结构，归纳核心要点，
  为每个主题生成符合特定风格的配图。支持封面图生成和自定义图片比例。
  使用场景：当用户需要为文档、文章、笔记生成配图时。
  关键词：配图、插图、illustration、generate images、document images
allowed-tools:
  - Read
  - Write
  - Bash(python:*)
  - Glob
  - AskUserQuestion
model: claude-sonnet-4-5-20250514
---

# Document Illustrator Skill

基于 AI 智能分析的文档配图生成工具。无需依赖特定格式，自动理解内容并生成专业配图。

## 🎯 核心特点

- ✨ **AI 智能归纳**：自动理解文档内容，智能提取核心主题
- 🎨 **格式无关**：支持任何格式的文档（Markdown、纯文本、PDF 等）
- 📐 **灵活比例**：支持 16:9（横屏）和 3:4（竖屏）
- 🖼️ **封面图可选**：可生成概括全文的封面图
- 🎭 **三种风格**：渐变玻璃卡片、票据风格、矢量插画

## 🚀 使用方法

### 直接告诉 Claude

```
帮我为这个文档生成配图：/path/to/document.md
```

或者：

```
我想为这篇文章生成一些配图
```

## 📝 完整工作流程

### 第 1 步：Claude 读取和理解文档

当你请求生成配图时，Claude 会：
1. 使用 Read 工具读取完整文档
2. AI 分析理解文档内容和结构
3. 识别核心主题和要点

**无需担心文档格式**：
- ✅ 标准 Markdown（##、###）
- ✅ 分隔线格式（======、------）
- ✅ 纯文本段落
- ✅ 任何其他格式

### 第 2 步：配置选项（3 个问题）

Claude 会询问你的偏好：

#### 问题 1：图片比例
```
请选择图片比例：
1. 16:9 (横屏) - 适合演示文稿、幻灯片、横屏展示
2. 3:4 (竖屏) - 适合社交媒体、手机查看、海报

请选择 (1/2):
```

#### 问题 2：封面图
```
是否生成封面图？
封面图将概括文档的所有核心信息，作为系列配图的引导。

1. 是 - 生成封面图 + 内容配图
2. 否 - 仅生成内容配图

请选择 (1/2):
```

#### 问题 3：内容配图数量
```
期望生成多少张内容配图？
建议范围：3-10 张
根据文档内容，推荐生成 6 张

请输入数字：
```

#
```

</details>
