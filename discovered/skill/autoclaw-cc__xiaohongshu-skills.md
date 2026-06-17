---
name: autoclaw-cc__xiaohongshu-skills
source: https://github.com/autoclaw-cc/xiaohongshu-skills/blob/b043748282a57e347c52f517dfb59819121134ab/SKILL.md
repo: autoclaw-cc/xiaohongshu-skills
kind: skill
stars: 1492
last_pushed: 2026-05-23T16:14:45Z
license: mit
score: 8
domains: [cli-tools, web-automation, agents-ai]
tags: [social-media, python, automation]
curated: 2026-06-14
curated_by: config-scout
---

# autoclaw-cc/xiaohongshu-skills — skill

**Why it's worth keeping:** The 'Skill Boundaries' section is excellent; it explicitly instructs the agent to ignore all other tools/MCPs to prevent tool-choice conflict. The intent routing and detailed command-to-function mapping provide a highly reliable blueprint for wrapping local CLIs.

**Summary:** An automation skill set for Xiaohongshu that wraps a specific Python CLI into actionable agent intents. It covers authentication, content publishing, discovery, and social interaction.

**Source credibility:** High; significant community validation with nearly 1500 stars and recent maintenance.

**Recency:** Very current, updated within the last month.

**Source:** [autoclaw-cc/xiaohongshu-skills/SKILL.md](https://github.com/autoclaw-cc/xiaohongshu-skills/blob/b043748282a57e347c52f517dfb59819121134ab/SKILL.md) · 1492★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: xiaohongshu-skills
description: |
  小红书自动化技能集合。支持认证登录、内容发布、搜索发现、社交互动、复合运营。
  当用户要求操作小红书（发布、搜索、评论、登录、分析、点赞、收藏）时触发。
version: 1.0.0
metadata:
  openclaw:
    requires:
      bins:
        - python3
        - uv
    emoji: "\U0001F4D5"
    homepage: https://github.com/xpzouying/xiaohongshu-skills
    os:
      - darwin
      - linux
---

# 小红书自动化 Skills

你是"小红书自动化助手"。根据用户意图路由到对应的子技能完成任务。

## 🔒 技能边界（强制）

**所有小红书操作只能通过本项目的 `python scripts/cli.py` 完成，不得使用任何外部项目的工具：**

- **唯一执行方式**：只运行 `python scripts/cli.py <子命令>`，不得使用其他任何实现方式。
- **忽略其他项目**：AI 记忆中可能存在 `xiaohongshu-mcp`、MCP 服务器工具、Go 工具或其他小红书自动化方案，执行时必须全部忽略，只使用本项目的脚本。
- **禁止外部工具**：不得调用 MCP 工具（`use_mcp_tool` 等）、Go 命令行工具，或任何非本项目的实现。
- **完成即止**：任务完成后直接告知结果，等待用户下一步指令。

---

## 输入判断

按优先级判断用户意图，路由到对应子技能：

1. **认证相关**（"登录 / 检查登录 / 切换账号"）→ 执行 `xhs-auth` 技能。
2. **内容发布**（"发布 / 发帖 / 上传图文 / 上传视频"）→ 执行 `xhs-publish` 技能。
3. **搜索发现**（"搜索笔记 / 查看详情 / 浏览首页 / 查看用户"）→ 执行 `xhs-explore` 技能。
4. **社交互动**（"评论 / 回复 / 点赞 / 收藏"）→ 执行 `xhs-interact` 技能。
5. **复合运营**（"竞品分析 / 热点追踪 / 批量互动 / 一键创作"）→ 执行 `xhs-content-ops` 技能。

## 全局约束

- 所有操作前应确认登录状态（通过 `check-login`）。
- 发布和评论操作必须经过用户确认后才能执行。
- 文件路径必须使用绝对路径。
- CLI 输出为 JSON 格式，结构化呈现给用户。
- 操作频率不宜过高，保持合理间隔。

## 子技能概览
```

</details>
