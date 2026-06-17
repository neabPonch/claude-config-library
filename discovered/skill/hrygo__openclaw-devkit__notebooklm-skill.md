---
name: hrygo__openclaw-devkit__notebooklm-skill
source: https://github.com/hrygo/openclaw-devkit/blob/9228a38b0675df0667f44fa0ed868ecf90932818/docs/NOTEBOOKLM_SKILL.md
repo: hrygo/openclaw-devkit
kind: skill
stars: 10
last_pushed: 2026-04-25T07:07:37Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, research-automation]
tags: [notebooklm, integration-pattern, authentication-sharing]
curated: 2026-06-17
curated_by: config-scout
---

# hrygo/openclaw-devkit — skill

**Why it's worth keeping:** Demonstrates sophisticated techniques for passing host-side authentication (cookies/storage_state) into containers; provides a highly structured command-to-task mapping essential for high-utility skills.

**Summary:** A detailed integration blueprint for bridging the NotebookLM CLI into an agentic environment through containerized volume mapping and authentication sharing.

**Source credibility:** Niche project with moderate activity (10 stars, updated 2 months ago).

**Recency:** Very current; aligns with modern agentic workflows and tool-use patterns.

**Source:** [hrygo/openclaw-devkit/docs/NOTEBOOKLM_SKILL.md](https://github.com/hrygo/openclaw-devkit/blob/9228a38b0675df0667f44fa0ed868ecf90932818/docs/NOTEBOOKLM_SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenClaw × NotebookLM 技能集成指南

本指南介绍如何在 OpenClaw DevKit 中集成和使用 Google NotebookLM CLI 技能，实现通过自然语言操控 NotebookLM 的全部功能。

## 目录

- [功能一览](#功能一览)
- [快速开始](#快速开始)
- [架构映射图](#架构映射图)
- [使用示例](#使用示例)
- [常用命令](#常用命令)
- [故障排除](#故障排除)

---

## 功能一览

**notebooklm-py** 是 Google NotebookLM 的非官方 Python SDK 和 CLI 工具，提供：

| 功能            | 说明                                           |
| :-------------- | :--------------------------------------------- |
| 📓 Notebook 管理 | 创建、列表、重命名、删除                       |
| 📄 多格式来源    | URLs、YouTube、PDF、Word、音视频、Google Drive |
| 💬 智能对话      | 基于来源的问答、自定义人设                     |
| 🔍 研究代理      | 网页/Drive 深度研究，自动导入                  |
| 🎙️ 内容生成      | 播客、视频、幻灯片、测验、思维导图等           |
| 📥 批量导出      | MP3、MP4、PDF、PNG、CSV、JSON、Markdown        |

> ⚠️ **注意**: 此工具使用未公开的 Google API，可能随时变化。适合原型开发、研究和个人项目。

---

## 快速开始

### Step 1: 宿主机安装 CLI

```bash
# 安装 CLI 工具
pip install "notebooklm-py[browser]"

# 安装浏览器（首次登录需要）
playwright install chromium
```

### Step 2: Google 认证

```bash
# 启动浏览器登录
notebooklm login
```

执行后会自动打开浏览器窗口。

#### ⚠️ 登录流程 - 务必按顺序操作

```
1. 浏览器打开 → 在浏览器中完成 Google 登录
2. 等待      → 看到 NotebookLM 首页（不是 Google 登录成功页面）
3. 回终端    → 按 ENTER 键保存认证
4. 完成      → 此时才能关闭浏览器
```

</details>
