---
name: xintaofei__nextbb
source: https://github.com/xintaofei/nextbb/blob/1bd968914693b9ed4e0d38715b29419b77e8c41b/Claude.md
repo: xintaofei/nextbb
kind: claude-md
stars: 40
last_pushed: 2026-02-27T16:41:55Z
license: gpl-2.0
score: 8
domains: [web-frontend, fullstack]
tags: [nextjs, typescript, prisma, tailwind-css]
curated: 2026-06-15
curated_by: config-scout
---

# xintaofei/nextbb — claude-md

**Why it's worth keeping:** It defines explicit guardrails for non-obvious tasks like BigInt handling, specific error response structures, and internationalization implementation rules.

**Summary:** A highly detailed technical specification for a Next.js/TypeScript fullstack application, covering schema patterns, API standards, and architectural constraints.

**Source credibility:** The repository has modest stars (40) but demonstrates high-quality, highly specific technical documentation.

**Recency:** Extremely current, utilizing Next.js 16 and Tailwind CSS 4.

**Source:** [xintaofei/nextbb/Claude.md](https://github.com/xintaofei/nextbb/blob/1bd968914693b9ed4e0d38715b29419b77e8c41b/Claude.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# NextBB 项目规范

## 概述

NextBB 是一个现代化的论坛应用，采用响应式设计，适配桌面端、平板和移动设备。

## 技术栈

- **框架**: Next.js 16
- **语言**: TypeScript（严格模式）
- **样式**: Tailwind CSS 4 + shadcn/ui
- **数据库**: Prisma ORM + PostgreSQL
- **认证**: NextAuth.js
- **数据请求**: SWR
- **国际化**: next-intl（never 模式，不使用路由前缀）
- **表单**: React Hook Form + Zod 4
- **包管理器**: pnpm

## 开发命令

### 基础命令

```bash
pnpm dev          # 启动开发服务器
pnpm build        # 构建生产版本（包含 prisma generate和数据库迁移）
pnpm build:code   # 只构建代码（包含 prisma generate）
pnpm lint         # 运行 ESLint 检查
```

### Prisma 命令

```bash
pnpm prisma:generate    # 生成 Prisma Client
pnpm prisma:validate    # 验证 Prisma schema
pnpm db:push            # 推送 schema 到数据库
pnpm db:pull            # 从数据库拉取 schema
```

## 代码风格

### TypeScript

- **严格模式**: 始终启用 TypeScript strict 模式
- **禁止 `any`**: 严禁使用 `any` 类型，请使用具体类型
- **显式类型**: 所有函数参数、返回值和变量都必须显式声明类型
- **BigInt**: 数据库 ID 使用 `bigint` 类型

### 格式化（Prettier）

```json
{
  "tabWidth": 2,
  "useTabs": false,
  "semi": false,
  "bracketSpacing": true,
  "trailingComma": "es5",
  "printWidth": 80
}
```

### 导入规范

- 使用 `@/` 别名导入 `src` 目录下的模块
- 外部库导入在前，内部模块导入在后

### 组件结构

- 使用 `memo` 优化性能
- Props 接口定义在组件外部
- 使用 `cn()` 工具函数合并 Tailwind 类名
- 使用 shadcn/ui 组件作为基础
```

</details>
