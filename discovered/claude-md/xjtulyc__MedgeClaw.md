---
name: xjtulyc__MedgeClaw
source: https://github.com/xjtulyc/MedgeClaw/blob/fef51d37ee3e1f5754790d9ae20f72c006c78dcc/CLAUDE.md
repo: xjtulyc/MedgeClaw
kind: claude-md
stars: 656
last_pushed: 2026-03-12T07:34:39Z
license: unknown
score: 9
domains: [bioinformatics, agents-ai, data-science, cli-tools]
tags: [docker, scientific-workflows, dashboard-driven, domain-specific-skills]
curated: 2026-06-15
curated_by: config-scout
---

# xjtulyc/MedgeClaw — claude-md

**Why it's worth keeping:** It excels at defining strict environmental boundaries (Docker vs Host), strict output path enforcement to prevent project clutter, and a 'skill-lookup' pattern where the AI must consult specialized documentation before acting.

**Summary:** A sophisticated operational manual for a biomedical research agent that manages execution within Docker and maintains real-time user visibility through a structured dashboard system.

**Source credibility:** High; 656 stars and highly specific technical constraints indicate a mature, functional research tool.

**Recency:** Current; specifically tailored for Claude Code and modern proxy environment configurations.

**Source:** [xjtulyc/MedgeClaw/CLAUDE.md](https://github.com/xjtulyc/MedgeClaw/blob/fef51d37ee3e1f5754790d9ae20f72c006c78dcc/CLAUDE.md) · 656★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - MedgeClaw Project Instructions

## Project Overview

MedgeClaw is a biomedical AI research assistant. You are the execution layer —
users describe analyses in natural language, and you write + run the code.

## 🔄 项目同步（重要）

**MedgeClaw 与 OpenClaw 的集成通过 `.medgeclaw-sync.yml` 配置文件管理。**

### 初始化/更新同步
```bash
cd <MedgeClaw项目目录>
python3 sync.py
openclaw gateway restart
```

### 同步内容
- 项目文档（MEDGECLAW.md, IDENTITY.md）→ OpenClaw workspace
- 自定义 skills → OpenClaw workspace/skills/
- SOUL.md / AGENTS.md 追加 MedgeClaw 身份段落
- openclaw.json 添加 MedgeClaw skills 路径

### 修改同步配置
编辑 `.medgeclaw-sync.yml`，无需改 `sync.py` 或 `medgeclaw-init.sh`。

## 📁 输出路径约束（重要）

**所有任务输出必须写入以下目录，不得写入项目根目录或其他位置：**

| 输出类型 | 路径 | 说明 |
|---------|------|------|
| 数据分析任务 | `data/<task_name>/output/` | CSV、图表、报告 |
| Dashboard | `data/<task_name>/dashboard/` | state.json, dashboard.html, serve.py |
| 科学写作 | `writing_outputs/<date>_<topic>/` | LaTeX、PDF、参考文献 |
| 临时文件 | `data/<task_name>/temp/` | 中间产物 |

**禁止写入：**
- ❌ 项目根目录
- ❌ `outputs/`（已废弃，仅保留兼容）
- ❌ OpenClaw workspace

**`.gitignore` 已配置忽略所有输出目录，确保不会误提交数据。**

## Execution Environment

**You run on the host, but execute code inside the Docker container.**

The an
```

</details>
