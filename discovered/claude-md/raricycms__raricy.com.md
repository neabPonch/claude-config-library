---
name: raricycms__raricy.com
source: https://github.com/raricycms/raricy.com/blob/1ce02350f0dbeebc52a58fe74fc76979d57c5b06/claude.md
repo: raricycms/raricy.com
kind: claude-md
stars: 2
last_pushed: 2026-06-15T05:02:28Z
license: mit
score: 9
domains: [web-backend, flask, python, frontend-architecture]
tags: [flask, architectural-guide, sc-structure, blueprint-mapping]
curated: 2026-06-16
curated_by: config-scout
---

# raricycms/raricy.com — claude-md

**Why it's worth keeping:** The use of structured tables for Blueprints and the explicit hierarchy for the SCSS layer provides excellent guardrails. It also documents specialized business logic like session versioning and role-based access which prevents AI-generated hallucinations regarding security/auth.

**Summary:** A highly detailed architectural blueprint for a Flask application, encompassing routing tables, model hierarchies, and strict SCSS organization rules.

**Source credibility:** A personal project with recent activity; the quality of documentation suggests a high degree of developer intentionality.

**Recency:** Extremely current; follows modern patterns for structured AI instructions.

**Source:** [raricycms/raricy.com/claude.md](https://github.com/raricycms/raricy.com/blob/1ce02350f0dbeebc52a58fe74fc76979d57c5b06/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
\# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

\## 项目概述

Flask 博客（raricy.com），Python 后端 + 原生前端（Jinja2 模板 + 静态 CSS/JS）。

\## 常用命令

\- 运行：python run.py

\- 依赖安装：pip install -r requirements.txt

\- 数据库迁移：flask db migrate -m "描述" / flask db upgrade

\- 管理员权限管理：flask promote-admin <username> / flask demote-admin <username>

\- 站长权限管理：flask promote-owner <username> / flask demote-owner <username>

\- 导入历史博客：flask import-blogs \[--overwrite]

\## 架构

\### 应用工厂

run.py → app/\_\_init\_\_.py:create\_app() 创建 Flask 实例，按顺序：加载配置 → 注册 Jinja2 过滤器/全局函数 → 注册蓝图 → 初始化扩展 → 注册 CLI 命令。

\### 配置

app/config.py — 通过 CONFIG\_TYPE 环境变量切换 DevelopmentConfig / ProductionConfig / TestingConfig。所有敏感配置（SECRET\_KEY、数据库 URI、Turnstile 密钥）均从 .env 读取。默认使用 instance/database/db.db 的 SQLite。

\### 蓝图（Blueprint）

在 app/web/\_\_init\_\_.py:register\_blueprints() 中统一注册：

| 蓝图 | URL 前缀 | 用途 |

|------|----------|------|

| home\_bp | / | 首页、robots.txt、联系页面、邀请码生成 |

| auth\_bp | /auth | 登录、注册、认证、资料、用户管理 |

| blog\_bp | /blog | 博客 CRUD、管理后台、API（点赞/评论）、爬虫 API |

| notifications\_bp | /notifications | 通知中心 |

| tool\_bp | /tool | 工具页面 |

| story\_bp | /story
```

</details>
