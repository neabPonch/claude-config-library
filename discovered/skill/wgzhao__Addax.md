---
name: wgzhao__Addax
source: https://github.com/wgzhao/Addax/blob/9175a65cadbc79a25e13201e3df9ceb834535bfd/SKILL.md
repo: wgzhao/Addax
kind: skill
stars: 1416
last_pushed: 2026-06-08T19:02:18Z
license: apache-2.0
score: 9
domains: [etl, data-engineering, cli-tools]
tags: [domain-knowledge, config-schema, mental-models]
curated: 2026-06-16
curated_by: config-scout
---

# wgzhao/Addax — skill

**Why it's worth keeping:** It demonstrates how to provide an AI with a 'mental model'—including specific mathematical relationships for concurrency and exact JSON structures—enabling it to move beyond simple code completion to complex troubleshooting.

**Summary:** A high-density domain knowledge file for the Addax ETL tool that maps out architectural hierarchies, JSON configuration schemas, and operational logic.

**Source credibility:** High-star (1.4k) active repository specializing in data movement.

**Recency:** Current; follows modern patterns of structured context injection for AI agents.

**Source:** [wgzhao/Addax/SKILL.md](https://github.com/wgzhao/Addax/blob/9175a65cadbc79a25e13201e3df9ceb834535bfd/SKILL.md) · 1416★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL: Addax 项目知识

## 1. 项目整体认识

### 1.1 项目定位

- **名称**：Addax  
- **类型**：通用开源 ETL 工具（Extract–Transform–Load）  
- **起源**：基于阿里巴巴 DataX 的 fork 与演进  
- **目标**：在多种异构数据源之间，提供稳定、高效、可扩展的“离线数据同步”能力

### 1.2 核心价值

- 支持 **20+ SQL/NoSQL/文件/时序/大数据** 数据源
- 使用 **JSON 任务配置** 即可完成复杂同步，无需写代码
- 插件化架构，Reader / Writer / Transformer 解耦，可自由扩展
- 提供 **数据质量监控、速率控制、错误容忍、脏数据探测** 等生产级能力
- 既可命令行运行，也可通过 **Server 模块 HTTP 接口** 异步提交和管理任务
- 有配套的 **addax-admin / addax-ui** 项目做 Web 管控

---

## 2. 概念与架构模型

### 2.1 核心业务概念

在与用户讨论 / 理解需求时，应优先按以下抽象模型理解：

- **Job（作业）**
  - 一次完整的数据同步任务，从一个源到一个目标
  - 通过一个 JSON 文件描述：数据源 reader、目标端 writer、变换规则、速率控制、错误阈值等
  - Job 是业务上的最小单位，如 “从 MySQL 表 A 同步到 PostgreSQL 表 B”

- **Task（子任务）**
  - 为提升性能，将一个 Job 拆分为多个 Task 并发执行
  - 每个 Task 负责同步一部分数据（如若干分表、某一范围分片）

- **TaskGroup**
  - 一组 Task 的集合，由框架统一调度执行
  - 每个 TaskGroup 内有若干通道（channel），每个 channel 负责一条 `Reader → Channel → Writer` 流水线

- **Reader 插件**
  - 数据采集模块，负责从“源数据源”读取数据，发送给框架
  - 只关心“如何正确读”，不关注类型转换、指标统计等通用问题

- **Writer 插件**
  - 数据写入模块，负责从框架拿数据写入“目标端”
  - 只关心“如何正确写”，通用逻辑由框架处理

- **Transformer（数据转换）**
  - 可选模块，在 Reader 和 Writer 之间对数据进行转换
  - 支持内置 UDF：`dx_substr` / `dx_pad` / `dx_replace` / `dx_filter` / `dx_groovy`
  - 可以做脱敏、字段裁剪、补全、过滤、自定义 G
```

</details>
