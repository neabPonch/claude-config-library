---
name: SenseTime-Copilot__raccoon-dataanalysis-skill
source: https://github.com/SenseTime-Copilot/raccoon-dataanalysis-skill/blob/ae3ee2bd1bf1b287f61e73d2c014582a43d865aa/SKILL.md
repo: SenseTime-Copilot/raccoon-dataanalysis-skill
kind: skill
stars: 177
last_pushed: 2026-03-16T01:58:07Z
license: unknown
score: 8
domains: [agents-ai, data-analysis, api-integration]
tags: [remote-interpreter, visualization, sense-time]
curated: 2026-06-14
curated_by: config-scout
---

# SenseTime-Copilot/raccoon-dataanalysis-skill — skill

**Why it's worth keeping:** It uses high-priority negative constraints to prevent local tool misuse and provides highly structured error handling/environment verification patterns that are easily transferable to any specialized skill.

**Summary:** Configures Claude Code as a remote interface for the Raccoon data analysis API, ensuring all computation occurs server-side rather than through local libraries.

**Source credibility:** Developed by SenseTime, a major AI company; has respectable star count and recent activity.

**Recency:** Recent (last pushed 3 months ago) and follows current agentic tool-use patterns.

**Source:** [SenseTime-Copilot/raccoon-dataanalysis-skill/SKILL.md](https://github.com/SenseTime-Copilot/raccoon-dataanalysis-skill/blob/ae3ee2bd1bf1b287f61e73d2c014582a43d865aa/SKILL.md) · 177★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: raccoon-dataanalysis
description: >
  Raccoon (小浣熊) Data Analysis - Remote code interpreter and data visualization service
  powered by SenseTime. Upload files (Excel, CSV, etc.) for AI-driven analysis, chart generation,
  and automated insights. Supports data analysis sessions, file upload/download, visualization,
  and multi-turn conversations. Keywords: raccoon, data analysis, code interpreter, visualization,
  小浣熊, 数据分析, 代码解释器, 数据可视化.
homepage: https://xiaohuanxiong.com
metadata:
  {
    "clawdbot":
      {
        "emoji": "🦝",
        "requires":
          {
            "bins": ["python3"],
            "env": ["RACCOON_API_HOST", "RACCOON_API_TOKEN"],
          },
        "primaryEnv": "RACCOON_API_TOKEN",
      },
  }
---

# 小浣熊数据分析 SKILL

你是小浣熊(Raccoon)数据分析的操作助手。你的职责是通过调用小浣熊远程 API 或者本技能相关脚本来完成用户的数据分析需求。

## !! 最高优先级行为规则 !!

**你必须严格遵守以下规则，不得违反：**

1. **禁止本地分析数据。** 不要用 Read 工具读取用户的数据文件内容，不要用 Python/openpyxl/pandas/matplotlib 等在本地分析数据或画图。你不是本地数据分析工具。
2. **所有数据分析工作必须交给小浣熊远程 API 完成。** 你的角色是：把用户的文件上传到小浣熊 → 把用户的需求发给小浣熊 → 把小浣熊返回的结果展示给用户。
3. **仅在用户当前请求明确要求使用本 Skill 时才开始工作。** 不要在 Skill 加载后自动调用 API。若用户明确要求分析或处理某个文件，可将该请求视为同意把该文件上传到用户配置的 `RACCOON_API_HOST`；若用户是否允许上传并不明确，先用一句话
```

</details>
