---
name: zstmfhy__zlibrary-to-notebooklm
source: https://github.com/zstmfhy/zlibrary-to-notebooklm/blob/4eb1f04a49e9bd2f846c26be4b025f8f9b9e7249/SKILL.md
repo: zstmfhy/zlibrary-to-notebooklm
kind: skill
stars: 1644
last_pushed: 2026-01-17T09:13:05Z
license: mit
score: 9
domains: [cli-tools, automation, web-scraping]
tags: [workflow, knowledge-management, automation]
curated: 2026-06-15
curated_by: config-scout
---

# zstmfhy/zlibrary-to-notebooklm — skill

**Why it's worth keeping:** Demonstrates excellent agentic patterns: explicit session management (storage_state.json), format fallback logic (PDF/EPUB), and proactive error recovery instructions.

**Summary:** Automates a multi-step workflow of downloading books via Playwright and uploading them to Google NotebookLM using specialized CLI commands.

**Source credibility:** High; 1600+ stars indicates significant community validation.

**Recency:** Current; reflects active development as of early 2025.

**Source:** [zstmfhy/zlibrary-to-notebooklm/SKILL.md](https://github.com/zstmfhy/zlibrary-to-notebooklm/blob/4eb1f04a49e9bd2f846c26be4b025f8f9b9e7249/SKILL.md) · 1644★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: zlibrary-to-notebooklm
description: 自动从 Z-Library 下载书籍并上传到 Google NotebookLM。支持 PDF/EPUB 格式，自动转换，一键创建知识库。
---

# Z-Library to NotebookLM Skill

让 Claude 帮你自动下载书籍并上传到 NotebookLM，实现"零幻觉"的 AI 对话式阅读。

## 🎯 核心功能

- 一键下载书籍（优先 PDF，自动降级 EPUB）
- 自动创建 NotebookLM 笔记本
- 上传文件并返回笔记本 ID
- 支持与 AI 进行基于书籍内容的对话

## 📋 激活条件（Triggers）

当用户提到以下需求时，使用此 Skill：

- 用户提供 Z-Library 书籍链接（包含 `zlib.li`、`z-lib.org`、`zh.zlib.li` 等域名）
- 用户说"帮我把这本书上传到 NotebookLM"
- 用户说"自动下载并读这本书"
- 用户说"用 Z-Library 链接创建 NotebookLM 知识库"
- 用户要求从特定 URL 下载书籍并分析

## 🔧 核心指令

当用户提供 Z-Library 链接时，按以下流程执行：

### Step 1: 提取信息

从用户提供的 URL 中提取：
- 书名
- 作者（如果有）
- 完整 URL
- 格式选项（PDF/EPUB/MOBI 等）

### Step 2: 自动下载

使用已保存的会话（`~/.zlibrary/storage_state.json`）自动登录 Z-Library：

1. **优先下载 PDF**（保留排版，AI 分析效果更好）
2. **自动降级**：如果没有 PDF，下载 EPUB
3. **格式转换**：如果下载 EPUB，使用 ebooklib 转换为纯文本

### Step 3: 创建 NotebookLM 笔记本

```bash
notebooklm create "书名"
```

### Step 4: 上传文件

```bash
notebooklm source add "文件路径"
```

### Step 5: 返回结果

向用户返回：
- ✅ 下载成功确认
- 📚 笔记本 ID
- 💡 建议的后续问题示例

### Step 6: 错误处理

如果遇到错误：
- 尝试重试最多 3 次
- 如果登录失败，提示用户运行 `python3 ~/.claude/skills/zlibrary-to-notebooklm/scripts/login.py`
- 如果下载失败，提供故障排查建议

## ⚠️ 重要限制

**仅限合法资源！**

- ✅ 用户拥有合法访问权限的资源
-
```

</details>
