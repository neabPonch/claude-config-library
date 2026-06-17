---
name: metowolf__vCards
source: https://github.com/metowolf/vCards/blob/fd6d46ca1cf6c1b2df536ef33ecc83eb3aa01f06/CLAUDE.md
repo: metowolf/vCards
kind: claude-md
stars: 6237
last_pushed: 2026-06-14T15:45:35Z
license: unknown
score: 9
domains: [data-processing, build-systems, cli-tools]
tags: [asset-management, data-validation, build-pipelines]
curated: 2026-06-15
curated_by: config-scout
---

# metowolf/vCards — claude-md

**Why it's worth keeping:** Provides explicit distinctions between similar build tasks; includes executable Python code snippets to handle rigid image size/format requirements which prevents agent error.

**Summary:** A highly detailed technical specification that covers build-system nuances, data validation schemas, and strict asset constraints. It includes actionable procedures for maintaining specific icon requirements.

**Source credibility:** High-star repository (6k+) with very active maintenance.

**Recency:** Extremely current, specifically mentions Claude Code and shows recent activity.

**Source:** [metowolf/vCards/CLAUDE.md](https://github.com/metowolf/vCards/blob/fd6d46ca1cf6c1b2df536ef33ecc83eb3aa01f06/CLAUDE.md) · 6237★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个中国常用联系人头像库（vCards），为 iOS/macOS 设备提供企业和机构的联系人信息，用于优化来电和信息界面体验。项目生成 vCard 格式的联系人文件，并支持通过 CardDAV 服务分发。

## 核心架构

### 数据结构
- `data/` - 按分类存储的 YAML 数据文件和对应的 PNG 图标
  - 每个条目包含一个 `.yaml` 配置文件和一个 `.png` 图标文件
  - YAML 文件包含 `basic` 对象，包含 `organization`、`cellPhone`、`url`、`workEmail` 等字段
  - 图标优先使用 512x512px（≤50KB），也支持 200x200px（≤20KB）的 PNG 格式

### 构建系统
- 使用 Gulp 作为构建工具，配置文件在 `src/gulpfile.js`
- 两个主要的生成流程：
  - `generator` - 标准 vCard 生成，过滤 106 开头的长号码（超过11位）
  - `generator_ext` - 扩展版本，保留所有号码并添加 git 历史时间戳
- 支持生成分类文件夹和汇总文件
- 支持生成 Radicale CardDAV 服务所需的文件结构
- 网页版本构建：`buildWeb` - 生成可浏览的网页界面

### 插件系统
- `src/plugins/vcard.js` - 标准 vCard 生成插件
- `src/plugins/vcard-ext.js` - 扩展版 vCard 生成插件，包含 REV 字段和 UID
- 使用 `vcards-js` 库生成 vCard 格式
- 自动添加拼音字段用于中文排序

## 常用命令

### 开发和测试
```bash
# 运行格式检查和数据验证
npm test
# 或使用 yarn
yarn test

# 构建标准版本（用于发布）
npm run build

# 构建 CardDAV 服务版本
npm run radicale

# 构建网页版本
npm run build:web

# 启动网页开发服务器
npm run dev:web
# 或单独启动服务器
npm run serve:web
```

### Gulp 任务
```bash
# 生成 vCard 文件到 temp 目录
npm run gulp generator

# 生成扩展版本 vCard（保留所有号码）
npm run gul
```

</details>
