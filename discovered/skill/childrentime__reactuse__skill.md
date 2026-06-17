---
name: childrentime__reactuse__skill
source: https://github.com/childrentime/reactuse/blob/d2b8cb2059e4912d898d721dbc1534a4f703b450/.claude/skills/medium-push/SKILL.md
repo: childrentime/reactuse
kind: skill
stars: 1015
last_pushed: 2026-05-27T12:38:04Z
license: unlicense
score: 8
domains: [cli-tools, web-automation]
tags: [markdown, medium, bridge-pattern, browser-interaction]
curated: 2026-06-15
curated_by: config-scout
---

# childrentime/reactuse — skill

**Why it's worth keeping:** Demonstrates a sophisticated 'Bridge Pattern' to overcome browser-only limitations; includes robust health checks and status verification (clientsSent) for reliable agent execution.

**Summary:** Automates the process of pushing local Markdown files into a Medium editor via a local Bridge server and a Chrome extension using SSE.

**Source credibility:** High technical sophistication, though the repository description provided seems unrelated to this specific skill file.

**Recency:** Highly relevant for modern agent workflows requiring local-to-browser automation.

**Source:** [childrentime/reactuse/.claude/skills/medium-push/SKILL.md](https://github.com/childrentime/reactuse/blob/d2b8cb2059e4912d898d721dbc1534a4f703b450/.claude/skills/medium-push/SKILL.md) · 1015★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: medium-push
category: publishing
description: 将 Markdown 文件推送到浏览器中打开的 Medium 编辑器。当用户说"发布到 medium"、"推送到 medium"、"paste to medium"、"push to medium"或在完成文章生成后要求发送到 Medium 时触发。
---

# medium-push - 推送 Markdown 到 Medium 编辑器

通过 Chrome 扩展 + Bridge 服务（HTTP + SSE），将本地 Markdown 文件转换为富文本并推送到浏览器中打开的 Medium 编辑器。

## 架构

```
Claude Code (读取 Markdown 文件)
  → curl POST http://localhost:18766/paste
    → Bridge Server (SSE 推送)
      → Chrome Extension (content script)
        → Markdown → HTML 转换
          → Medium 编辑器 (模拟粘贴富文本)
```

## 工作流程

### 步骤 1：检查 Bridge 服务

```bash
curl -s http://localhost:18766/health 2>/dev/null || echo "NOT_RUNNING"
```

| 结果 | 操作 |
|------|------|
| `{"status":"ok",...}` | Bridge 已运行，跳到步骤 2 |
| `NOT_RUNNING` | 启动 Bridge 服务 |

**启动 Bridge：**

```bash
nohup node <skill-path>/scripts/bridge.mjs > /tmp/medium-push-bridge.log 2>&1 &
echo $!
```

等待 1 秒后再次检查 `/health` 确认启动成功。

### 步骤 2：确认 Medium 编辑器已打开

提示用户在 Chrome 中打开 Medium 新文章页面：

```
https://medium.com/new-story
```

### 步骤 3：读取 Markdown 文件

读取用户指定的 Markdown 文件路径。如果用户没有指定，查找 `blog-external/` 目录下的 `medium.md` 文件。

### 步骤 4：发送到 Medium 编辑器

**方式 A：通过文件路径（推荐）**

```bash
curl -s -X POST http://localhost:18766/paste
```

</details>
