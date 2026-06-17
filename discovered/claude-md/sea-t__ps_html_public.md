---
name: sea-t__ps_html_public
source: https://github.com/sea-t/ps_html_public/blob/502f05cbd54992f764e682e6110d7f28bd72cff9/Claude.md
repo: sea-t/ps_html_public
kind: claude-md
stars: 0
last_pushed: 2025-11-20T13:01:40Z
license: unknown
score: 8
domains: [web-frontend, devops, agents-ai]
tags: [agentic-workflow, pr-automation, github-cli]
curated: 2026-06-14
curated_by: config-scout
---

# sea-t/ps_html_public — claude-md

**Why it's worth keeping:** The 'AI Agent Behavior Norms' section is a high-value pattern; it moves beyond instructions to specific behavioral protocols. It also documents internal parsing logic (regex/logic) so the agent can safely maintain data conversion scripts.

**Summary:** Implements a specialized 'agentic workflow' that forces the AI to proactively generate Pull Request links and handles tool permissions for GitHub CLI.

**Source credibility:** Low star count, but the documentation quality suggests a highly structured personal automation setup.

**Recency:** Current; uses modern patterns for GitHub CLI integration and Claude Code tool usage.

**Source:** [sea-t/ps_html_public/Claude.md](https://github.com/sea-t/ps_html_public/blob/502f05cbd54992f764e682e6110d7f28bd72cff9/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - PS HTML Public 项目文档

> 本文档帮助 AI 快速理解 ps_html_public 项目的架构、功能和工作流程

## ⚠️ AI Agent 行为规范

### 自动化 PR 链接输出

**重要规则：** 当完成任务实现、代码提交并推送后，**必须主动输出** PR 创建链接，无需等待用户询问。

**输出格式：**
```
✅ 任务已完成并推送！

📝 创建 Pull Request：
https://github.com/sea-t/ps_html_public/pull/new/{当前分支名}

点击上方链接即可创建 PR
```

**触发条件：**
- 完成代码实现
- 已执行 `git commit`
- 已执行 `git push`

**示例：**
如果当前分支是 `claude/feature-abc-123`，则自动输出：
```
✅ 任务已完成并推送！

📝 创建 Pull Request：
https://github.com/sea-t/ps_html_public/pull/new/claude/feature-abc-123
```

## 项目概述

**ps_html_public** 是一个轻量级的 HTML 导航页面项目，具备完整的自动化工程实践。项目采用纯原生技术栈（无框架依赖），展示了现代 Web 开发和 DevOps 自动化的最佳实践。

### 核心特点

- **前端应用**：响应式导航页面，支持分类展示和实时搜索
- **数据管理**：Markdown 源文件自动转换为 JSON 数据
- **自动化工程**：完整的 CI/CD 流程，自动化分支管理
- **无依赖设计**：前端零外部依赖，纯原生 HTML/CSS/JavaScript
- **开发友好**：集成 Claude Code，支持 AI 辅助开发

### 技术栈

| 类别 | 技术 |
|------|------|
| 前端 | HTML5, CSS3, JavaScript (ES6+) |
| 后端/脚本 | Node.js, Shell/Bash |
| 版本控制 | Git, GitHub |
| CI/CD | GitHub Actions |
| AI 工具 | Claude Code |

## 项目结构

```
ps_html_public/
├── .claude/                              # Claude Code 配置
│   ├── settings.json                     # Claude 权限设置
│   └── README.md                         # Claude 配
```

</details>
