---
name: wasabeef__claude-code-cookbook__skill
source: https://github.com/wasabeef/claude-code-cookbook/blob/d4a413b713119573fce72b49d111a1dd2bbc0b91/plugins/zh-cn/skills/task/SKILL.md
repo: wasabeef/claude-code-cookbook
kind: skill
stars: 1103
last_pushed: 2026-04-15T03:12:12Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, devops]
tags: [autonomous-agent, investigation, research]
curated: 2026-06-15
curated_by: config-scout
---

# wasabeef/claude-code-cookbook — skill

**Why it's worth keeping:** Provides a clear decision matrix to distinguish investigation from planning/thinking, and defines structured workflows for complex technical audits.

**Summary:** Creates a specialized 'Task' persona designed for autonomous, multi-step research and analysis using local files and web tools.

**Source credibility:** High; part of a popular, well-maintained Claude Code cookbook.

**Recency:** Current; utilizes modern toolsets like WebSearch and WebFetch typical of current agentic CLI capabilities.

**Source:** [wasabeef/claude-code-cookbook/plugins/zh-cn/skills/task/SKILL.md](https://github.com/wasabeef/claude-code-cookbook/blob/d4a413b713119573fce72b49d111a1dd2bbc0b91/plugins/zh-cn/skills/task/SKILL.md) · 1103★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: "专用代理自主执行调查分析任务。「用 Task 调查」「调查一下」「分析一下」「搜索」等触发。"
allowed-tools:
  - Read
  - Grep
  - Glob
  - Bash
  - WebSearch
  - WebFetch
---

# 专用代理自主执行调查分析任务

启动专用代理，自主执行复杂的搜索、调查和分析任务。通过组合多个工具进行大规模信息处理，重视上下文效率。

## 使用方法

```bash
# 向 Claude 请求 Task
「用 Task 调查[课题]」
```

## Task 的特点

**自主执行**

- 自动组合多个工具执行
- 分阶段信息收集和分析
- 结果整合和结构化报告

**高效信息处理**

- 优化上下文消耗
- 大规模文件搜索和解析
- 从外部信息源收集数据

**质量保证**

- 信息源可靠性检查
- 多角度验证
- 自动补充缺失信息

## 基本示例

```bash
# 复杂代码库调查
「用 Task 调查这个功能在哪些文件中实现」

# 大规模文件搜索
「用 Task 识别配置文件的不一致」

# 外部信息收集
「用 Task 调查最新的 AI 技术趋势」
```

## 与 Claude 配合

```bash
# 复杂问题分析
「用 Task 分析内存泄漏的原因。包括性能分析结果和日志」

# 依赖关系调查
「用 Task 调查这个 npm 包的漏洞」

# 竞品分析
「用 Task 调查竞品服务的 API 规格」

# 架构分析
「用 Task 分析这个微服务的依赖关系」
```

## 与其他命令的区别

### Task vs 其他命令

| 命令                | 主要用途         | 执行方式   | 信息收集       |
| ------------------- | ---------------- | ---------- | -------------- |
| **Task**            | 调查・分析・搜索 | 自主执行   | 多源           |
| ultrathink          | 深度思考・判断   | 结构化思考 | 以现有知识为主 |
| sequential-thinking | 问题解决・设计   | 分阶段思考 | 按需           |
| plan                | 制定实施计划     | 批准流程   | 需求分析       |

### 判断流程图

```text
需要信息收集？
├─ Yes → 多源・大规模？
│          ├─ Yes → **Task**
│          └─ No →
```

</details>
