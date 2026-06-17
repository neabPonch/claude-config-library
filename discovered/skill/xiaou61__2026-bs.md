---
name: xiaou61__2026-bs
source: https://github.com/xiaou61/2026-bs/blob/12c74826d29da2a9e18554558ad09f198e9e183c/skill.md
repo: xiaou61/2026-bs
kind: skill
stars: 97
last_pushed: 2026-06-01T12:40:57Z
license: unknown
score: 8
domains: [fullstack, java, web-development]
tags: [workflow, orchestration, step-by-step]
curated: 2026-06-14
curated_by: config-scout
---

# xiaou61/2026-bs — skill

**Why it's worth keeping:** It defines explicit file creation sequences to prevent dependency errors and includes detailed quality check-lists for the agent to validate its own output.

**Summary:** A rigorous orchestration workflow for full-stack development (Spring Boot + Vue) that guides an agent through structured planning and execution stages.

**Source credibility:** The source is a niche repository of student projects, but the workflow logic demonstrates high level of instructional design.

**Recency:** Current; utilizes modern frameworks like Vue 3/Vite and integrates with tool-calling workflows.

**Source:** [xiaou61/2026-bs/skill.md](https://github.com/xiaou61/2026-bs/blob/12c74826d29da2a9e18554558ad09f198e9e183c/skill.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 毕设项目开发工作流程

## 📋 完整流程概览

```
1. 读取规则 → 2. 编写PRD → 3. 制定Plan → 4. 后端实现 → 5. 前端实现 → 6. 更新README
```

---

## 🔄 详细步骤

### Step 1: 读取项目规则
**目的**: 了解项目约束和技术栈要求

**操作**:
```
读取 rule.md 文件，记住以下要点：
- 不写注释
- 不写README（除非明确要求）
- 不进行编译验证
- Windows环境
- 前端不使用npx命令
- 技术栈：MyBatis/MyBatis-Plus + Redis + Vue + SpringBoot
```

---

### Step 2: 编写PRD文档
**目的**: 明确需求和技术设计

**文件位置**: `项目目录/PRD.md`

**内容结构**:
```markdown
# 项目标题

## 项目概述
- 项目简介
- 核心功能
- 技术栈

## 功能需求
### 1. 模块一
- 功能点1
- 功能点2

### 2. 模块二
...

## 技术设计
### 数据库设计
表1: xxx
- 字段列表
- 索引

### API接口设计
#### 1.1 接口名
- 请求方式: POST/GET
- 路径: /api/xxx
- 参数: {}
- 返回: {}

### 项目结构
后端:
```
backend/
├── src/main/java/com/xxx/
│   ├── entity/
│   ├── mapper/
│   ├── service/
│   └── controller/
```

前端:
```
frontend/
├── src/
│   ├── views/
│   ├── api/
│   └── router/
```

## 用户角色
- 角色1: 权限描述
- 角色2: 权限描述

## 默认账号
- admin/123456
- user/123456
```

---

### Step 3: 制定实施计划
**目的**: 规划实现步骤

**操作**:
```
使用 create_plan 工具创建计划
```

**计划内容**:
```markdown
# 实现计划

## 问题陈述
简述项目背景和要解决的问题

## 当前状态
已有的项目结构和文件

## 实施方案

### 第一阶段: 后端开发
1. 基础架构
   - pom.xml配置
   - application.yml配置
   - 启动类
   - 通用模块(Result/Exception/JWT)

2. 数据库
   - 创建init.sql
   - 12张表结构

3. 实体类
   - 所有Ent
```

</details>
