---
name: gugug168__cute-claude-hooks
source: https://github.com/gugug168/cute-claude-hooks/blob/3fff99dcc02517849a5675ba783cf555bfabb74c/SKILL.md
repo: gugug168/cute-claude-hooks
kind: skill
stars: 205
last_pushed: 2026-05-23T08:11:30Z
license: mit
score: 7
domains: [cli-tools, ux-enhancement]
tags: [hooks, observability, localization]
curated: 2026-06-15
curated_by: config-scout
---

# gugug168/cute-claude-hooks — skill

**Why it's worth keeping:** Demonstrates a specific pattern for using 'PostToolUse' hooks to parse command arguments via shell and return descriptive system messages for better agent observability.

**Summary:** Enhances the Claude Code CLI by using shell hooks to intercept tool executions and inject human-readable command explanations and localized descriptions.

**Source credibility:** Strong community interest with 205 stars; recently maintained.

**Recency:** Highly current, updated within the last month.

**Source:** [gugug168/cute-claude-hooks/SKILL.md](https://github.com/gugug168/cute-claude-hooks/blob/3fff99dcc02517849a5675ba783cf555bfabb74c/SKILL.md) · 205★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cute-claude-hooks (可爱提示钩子)
description: 为 Claude Code 提供完整的中文体验！包含工具提示、界面汉化、完整的自定义指南、实战经验和进阶开发教程, 让用户能够根据自己的需求修改和完善.
---

# 🌸 Cute Claude Hooks - 完整指南
让 Claude Code 显示可爱的中文提示和界面!
---

---

## 📚 目录
0. [⚠️ 重要警告 - 必读！](#️-重要警告---必读)
1. [功能介绍](#-功能介绍)
2. [快速安装](#-快速安装)
3. [界面汉化](#-界面汉化)
4. [基础自定义](#-基础自定义)
5. [进阶自定义](#-进阶自定义)
6. [添加新功能](#-添加新功能)
7. [调试技巧](#-调试技巧)
8. [实战经验](#-实战经验)
9. [常见需求示例](#-常见需求示例)
10. [问题排查](#-问题排查)
11. [文件位置速查](#-文件位置速查)
12. [恢复默认](#-恢复默认)
13. [相关资源](#-相关资源)
14. [汉化关键词表](#-汉化关键词表)
15. [常见问题](#-常见问题)
16. [技术说明](#-技术说明)
17. [更新日志](#-更新日志)
18. [贡献指南](#-贡献指南)
19. [许可证](#-许可证)

---

## ⚠️ 重要警告 - 必读！

### 🚫 不要随意修改的关键短语

在自定义钩子脚本时，**以下短语/格式千万不能随意修改**，否则可能导致 Claude Code 无法正常启动或运行：

| 类型 | 不能修改的内容 | 原因 |
|------|---------------|------|
| **JSON 结构** | `{"systemMessage":"..."}` 格式 | Claude Code 依赖此格式解析 hook 输出 |
| **特殊标记** | `<{{GUID}}>` 格式的标记 | 系统内部通信标识符 |
| **工具名称** | `Bash`, `Read`, `Write` 等工具名 | 与 Claude Code 内部工具对应 |
| **钩子字段** | `PreToolUse`, `PostToolUse` 等事件名 | 钩子系统核心字段 |
| **环境变量名** | `CLAUDE_CODE_*` 相关变量 | 系统运行时依赖 |

### 💡 修改时的安全原则

1. **只修改显示文本** - 例如工具提示的中文名
2. **保持 JSON 结构完整** - 不要删除或重命名字段
3. **测试后再使用** - 修改后先用简单命令测试
4. **保留备份** - 修改前备份原始文件

### 🔧 C
```

</details>
