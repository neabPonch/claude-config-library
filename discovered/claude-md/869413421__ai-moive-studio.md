---
name: 869413421__ai-moive-studio
source: https://github.com/869413421/ai-moive-studio/blob/28b011b8e434a3aa065f0f0aa877b2f22eb5efd3/CLAUDE.md
repo: 869413421/ai-moive-studio
kind: claude-md
stars: 1242
last_pushed: 2026-04-06T05:41:44Z
license: apache-2.0
score: 8
domains: [full-stack, web-development, backend-api, frontend]
tags: [fastapi, vue3, architectural-patterns, devops]
curated: 2026-06-14
curated_by: config-scout
---

# 869413421/ai-moive-studio — claude-md

**Why it's worth keeping:** Provides specific business logic rules (timezone standards, error handling nuances) and clear structural hierarchies that help an agent understand the 'why' behind code patterns, not just the 'how'.

**Summary:** A high-quality full-stack guide covering a FastAPI backend and Vue frontend, including database migrations, architectural patterns, and environment setup.

**Source credibility:** High credibility; highly starred repository with recent updates.

**Recency:** Very current; utilizes modern tooling like `uv` for Python dependency management.

**Source:** [869413421/ai-moive-studio/CLAUDE.md](https://github.com/869413421/ai-moive-studio/blob/28b011b8e434a3aa065f0f0aa877b2f22eb5efd3/CLAUDE.md) · 1242★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

AICG内容分发平台是一个AI驱动的长文本到视频自动转换系统，包含完整的前后端架构、用户管理系统、文件存储和异步任务处理功能。

## 开发环境设置

### 基础设施启动
```bash
./scripts/start.sh
```

### 后端开发
```bash
cd backend
uv sync                          # 安装依赖
alembic upgrade head             # 数据库迁移
uvicorn src.main:app --reload --host 0.0.0.0 --port 8000  # 开发服务器
```

### 前端开发
```bash
cd frontend
npm install                     # 安装依赖
npm run dev                     # 开发服务器（默认端口3000，会自动检测占用）
```

### 服务地址
- API文档: http://localhost:8000/docs
- MinIO控制台: http://localhost:9001 (minioadmin/minioadmin)
- 前端应用: http://localhost:3001 或 http://localhost:3000

## 项目架构

### 后端架构 (FastAPI + SQLAlchemy + Alembic)

**核心模块结构:**
- `src/core/`: 核心配置、数据库、安全、日志
- `src/models/`: SQLAlchemy数据模型（基于BaseModel的时间戳混入）
- `src/api/v1/`: API路由，按功能模块组织
- `src/services/`: 业务逻辑层，包括头像上传等服务
- `migrations/`: Alembic数据库迁移文件

**重要设计模式:**
- 使用异步SQLAlchemy (AsyncSession)
- 模型继承BaseModel（UUID主键 + 时间戳混入）
- 配置使用Pydantic Settings，支持环境变量覆盖
- JWT认证 + Bearer Token授权
- 统一的错误处理和响应格式

### 前端架构 (Vue 3 + Element Plus + Pinia)

**核心结构:**
- `src/router/`: 路由配置，包含认证守卫
- `src/store
```

</details>
