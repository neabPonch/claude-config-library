---
name: Colin4k1024__tsp__data-ml-pipeline-claude
source: https://github.com/Colin4k1024/tsp/blob/d4dbfc0d179a5c4d0be745f114a066f048420da0/examples/data-ml-pipeline-CLAUDE.md
repo: Colin4k1024/tsp
kind: claude-md
stars: 0
last_pushed: 2026-06-12T09:37:39Z
license: mit
score: 8
domains: [data-engineering, mlops, data-pipelines]
tags: [data, ml, etl, pipeline]
curated: 2026-06-14
curated_by: config-scout
---

# Colin4k1024/tsp — claude-md

**Why it's worth keeping:** It introduces critical domain-specific constraints like backfill scope, data lineage, and cost windows into the agent's verification process.

**Summary:** A highly specialized configuration for Data and ML pipelines that pivots focus from code logic to data integrity and orchestration.

**Source credibility:** Low star count/new repo; likely a template or experimental harness rather than established software.

**Recency:** Very current with modern agentic command patterns.

**Source:** [Colin4k1024/tsp/examples/data-ml-pipeline-CLAUDE.md](https://github.com/Colin4k1024/tsp/blob/d4dbfc0d179a5c4d0be745f114a066f048420da0/examples/data-ml-pipeline-CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Example Data ML Pipeline CLAUDE.md

适用于数据处理流水线、特征工程仓库、训练 / 推理 pipeline 仓库、批处理编排仓库或数据质量治理平台。

这类项目的重点不是单个页面，而是数据输入、转换链、质量校验、调度依赖、成本窗口和产物可追溯性。

## 适用信号

- 需求经常涉及数据抽取、清洗、特征、训练任务、推理任务、调度、回填或质量告警
- 成功标准常常是任务稳定、数据质量达标、成本可控和结果可追溯
- 项目通常同时关心批处理窗口、失败重跑、下游影响和 release 基线

## 相对通用版的主要差异

### 1. 命令流更强调验证闭环与结果回写

- 建议链路：`/team-intake` -> `/team-plan` -> `/tdd` -> `/team-execute` -> `/verify` -> `/team-review` -> `/team-release`
- 如果平台本身同时维护评测或调度能力，可按需补 `/harness-audit`

### 2. 项目约束更偏数据质量、批处理窗口和回填风险

- 必须说明输入源、转换边界、回填范围、失败重试和下游影响
- 验证不能只看任务完成，还要看数据质量、样本异常和成本窗口
- 产物、数据版本和关键结果必须可追溯

### 3. 角色链路更偏架构、后端 / 数据与 QA

- 默认保留：`tech-lead`、`architect`、`backend-engineer`、`qa-engineer`
- 若有运营台或配置台，再引入 `frontend-engineer`
- 若调度、环境和发布复杂，再引入 `devops-engineer`

## 一份更适合数据 / ML pipeline 仓库的精简成品

````md
# Data ML Pipeline Working Agreement

## 项目定位

- 类型：数据 / ML pipeline 仓库
- 重点：输入源、转换链、质量校验、调度依赖、成本窗口、结果追溯

## 默认角色

- `tech-lead`
- `architect`
- `backend-engineer`
- `qa-engineer`

## 默认命令流

1. `/team-intake`
2. `/team-plan`
3. `/tdd`
4. `/team-execute`
5. `/verify`
6. `/team-review`
7. `/team-release`

## 项目约束

- 必须写清输入源、数据口径、失败重试、回填边界和下游影响
- 验证不仅检查任务完成，还要检查数据质量、异常样本和成本窗口
- review / release 需要记录数据版本、任务窗口和关键结果摘要

#
```

</details>
