---
name: WJZ-P__gemini-skill
source: https://github.com/WJZ-P/gemini-skill/blob/9dbfd22adfb0a815bc9905eef78d569f7c86347b/SKILL.md
repo: WJZ-P/gemini-skill
kind: skill
stars: 823
last_pushed: 2026-06-12T12:55:36Z
license: mit
score: 9
domains: [agents-ai, web-automation, mcp]
tags: [gemini, image-generation, browser-control]
curated: 2026-06-14
curated_by: config-scout
---

# WJZ-P/gemini-skill — skill

**Why it's worth keeping:** It implements critical 'agent-to-tool' protocols: handling long-running tasks with explicit timeouts/heartbeats, enforcing operational priorities to prevent session conflicts, and providing diagnostic routines like page probing.

**Summary:** A sophisticated instruction set for an agent to control a Gemini web session via MCP, specifically optimized for image generation and chat automation.

**Source credibility:** Highly credible source with high star count (823) and very recent maintenance.

**Recency:** Extremely current; specifically tailored for modern MCP-capable agents and web automation needs.

**Source:** [WJZ-P/gemini-skill/SKILL.md](https://github.com/WJZ-P/gemini-skill/blob/9dbfd22adfb0a815bc9905eef78d569f7c86347b/SKILL.md) · 823★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gemini-skill
description: 通过 Gemini 官网（gemini.google.com）执行生图、对话等操作。用户提到"生图/画图/绘图/nano banana/nanobanana/生成图片"等关键词时触发。操作方式分三级优先级：首选 MCP 工具 → 次选 Skill 脚本 → 最次连接 Skill 浏览器手动操作（需用户授权）。禁止自行启动外部浏览器访问 Gemini。
---

# Gemini Skill

## ⚠️ 操作优先级（必须遵守）

与 Gemini 的一切交互，按以下优先级选择方式：

1. **🥇 首选：调用 MCP 工具** — 直接调用本 Skill 暴露的 MCP 工具完成操作，覆盖绝大多数场景
2. **🥈 次选：运行 Skill 脚本** — 当 MCP 工具无法满足需求时，可运行本 Skill 项目中提供的脚本来完成
3. **🥉 最次：连接 Skill 管理的浏览器** — 仅当前两种方式都无法解决时，可通过 `gemini_browser_info` 获取 CDP 连接信息，主动连接到本 Skill 管理的浏览器进行操作。**此方式必须先征得用户同意**

**绝对禁止**：自行启动新的浏览器实例访问 Gemini 页面（如使用 OpenClaw 浏览器、另起 Puppeteer 等），这会导致会话冲突。

> 浏览器 Daemon 未运行时 MCP 工具会自动拉起，无需任何手动操作。

## 📡 进度同步 & 长耗时工具规则

MCP 工具调用（尤其是生图、等待回复等）可能耗时较长（60~180 秒）。必须遵守以下规则：

- **本 Skill 所有 MCP 工具均为同步阻塞调用**，会等到最终结果才返回。不存在"中间状态"需要轮询。
- 调用长耗时工具时，`timeoutMs` 必须设为 ≥180000（3 分钟），避免传输层提前超时截断。
- **禁止在未收到工具最终返回前结束对话**或向用户报告"还在运行"/"工具超时"。
- 每隔 15~30 秒向用户发送一条进度消息（如"正在等待 Gemini 生成图片…已等待 30 秒…"），保持反馈。
- 拿到最终结果后**立即**回传产物（文件路径）或报告错误，不得遗漏。
- 若 `fullSize` 模式失败，可降级重试 `fullSize=false`（预览图模式更稳定）。

## 触发关键词

- **生图任务**：`生图`、`画`、`绘图`、`海报`、`nano banana`、`nanobanana`、`image generation`、`生成图片`
- 若请求含糊，先确认用户是否需要生图

## 使用方式

本 Skill 通过 MCP Server 暴露工具，AI 直接调用即可。

浏览器启动、会话管理
```

</details>
