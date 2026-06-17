---
name: creeper-RedWHU__HuaweiCloudProj__qa-skill
source: https://github.com/creeper-RedWHU/HuaweiCloudProj/blob/575c6e83a0703e19a7c8663bc3c242873dbd2f56/QA_SKILL.md
repo: creeper-RedWHU/HuaweiCloudProj
kind: skill
stars: 0
last_pushed: 2026-05-22T02:07:44Z
license: unknown
score: 8
domains: [web-frontend, security, quality-assurance, automation]
tags: [qa, playwright, xss-testing, test-driven]
curated: 2026-06-15
curated_by: config-scout
---

# creeper-RedWHU/HuaweiCloudProj — skill

**Why it's worth keeping:** The use of highly granular, categorized test matrices (Functional, Security/XSS, Boundary) provides an agent with precise execution vectors rather than vague goals. It also includes ready-to-use Playwright automation snippets that bridge the gap from planning to action.

**Summary:** A comprehensive QA skill that defines the architecture, data structures, and exhaustive test matrices for a specific web application.

**Source credibility:** Low; zero stars and a generic repository name suggest it is a private or specialized project file.

**Recency:** Current; uses modern testing stacks (Playwright, Node ESM).

**Source:** [creeper-RedWHU/HuaweiCloudProj/QA_SKILL.md](https://github.com/creeper-RedWHU/HuaweiCloudProj/blob/575c6e83a0703e19a7c8663bc3c242873dbd2f56/QA_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: qa
description: |
  任务管理看板 质量测试技能。对 http://119.3.174.235/ 执行全链路质量核验，
  涵盖功能验证、安全渗透、边界探索、异常恢复、性能评估、兼容性检测。
  触发词：测试、QA、质量、用例、回归、安全测试、测试报告。
---

# 任务管理看板 — 质量测试技能

你是资深 QA 工程师，负责对「任务管理看板」执行系统化质量测试并输出可追溯的测试证据。

## 被测系统

| 维度 | 详情 |
|------|------|
| URL | http://119.3.174.235/ |
| 标题 | 任务管理看板 |
| 架构 | Vue 3 SPA (Vite 构建)，纯前端无后端 |
| 存储 | localStorage，key=`task-kanban-data` |
| 路由 | 单页，无路由切换 |
| 认证 | 无，公开访问 |

## 功能全景

### 看板结构
- 三列：**待办** (todo) / **进行中** (doing) / **已完成** (done)
- 每列显示任务卡片列表 + 列标题 + 任务计数

### 任务实体
| 字段 | 类型 | 必填 | 长度限制 | 说明 |
|------|------|------|----------|------|
| id | string | 自动 | — | 唯一标识，程序生成 |
| title | string | 是 | maxlength=100 | 任务标题 |
| description | string | 否 | maxlength=500 | 任务描述，多行文本 |
| category | string | 否 | maxlength=20 | 自定义分类标签 |
| columnId | enum | 是 | — | todo / doing / done |
| starred | boolean | 否 | — | 星标标记 |
| urgent | boolean | 否 | — | 紧急标记 |
| createdAt | number | 自动 | — | Unix 时间戳 |

### 交互操作
1. **新增任务**: 模态框表单，标题必填（HTML5 required），其余选填
2. **删除任务**: 卡片 × 按钮，即时生效无确认
3. **星标切换**: 卡片 ★ 按钮，切换 `starred` 状态
4. **紧急切换**: 卡片 ! 按钮，切换 `urgent` 状态
5. **拖拽移动**: 卡片可在三列间拖拽，更新 `columnId`
6. **重置**: 清除全部数据，带 confirm 确认弹窗
7. **ESC 关闭**: 模态框支持
```

</details>
