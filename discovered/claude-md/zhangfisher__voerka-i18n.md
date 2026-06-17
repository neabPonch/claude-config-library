---
name: zhangfisher__voerka-i18n
source: https://github.com/zhangfisher/voerka-i18n/blob/2d270a3f728f6820797d7e9c06430a396c51aeb2/CLAUDE.md
repo: zhangfisher/voerka-i18n
kind: claude-md
stars: 223
last_pushed: 2026-02-11T08:21:00Z
license: mit
score: 8
domains: [cli-tools, web-frameworks, monorepo]
tags: [monorepo, i18n, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# zhangfisher/voerka-i18n — claude-md

**Why it's worth keeping:** Clearly outlines distinct development workflows for different module types (CLI vs. Adapters) within a complex workspace architecture.

**Summary:** Provides a comprehensive architectural map of the monorepo and essential command sets for package management.

**Source credibility:** High; based on a well-starred, actively maintained open-source project.

**Recency:** Current; utilizes modern toolchains like Turbo and pnpm workspaces.

**Source:** [zhangfisher/voerka-i18n/CLAUDE.md](https://github.com/zhangfisher/voerka-i18n/blob/2d270a3f728f6820797d7e9c06430a396c51aeb2/CLAUDE.md) · 223★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

VoerkaI18n 是一个为 JavaScript/TypeScript/Vue/React/Solidjs/SvelteJs/ReactNative 设计的国际化解决方案，提供全流程工程支持，包括文本提取、自动翻译、编译和动态语言切换。

## 核心架构

这是一个 monorepo 项目，使用 Turbo 进行构建管理，包含以下核心包：

- **@voerkai18n/runtime**: 核心运行时，提供 i18n 管理器、作用域、存储等功能
- **@voerkai18n/cli**: 命令行工具，用于初始化、提取、编译、自动翻译等
- **@voerkai18n/utils**: 工具函数库
- **@voerkai18n/formatters**: 格式化器
- **@voerkai18n/[framework]**: 各框架适配器 (vue, vue2, react, solid, svelte, astro, nextjs 等)
- **@voerkai18n/[tools]**: 构建工具集成 (babel, webpack, plugins)

## 常用命令

### 项目管理
```bash
# 安装依赖
pnpm install

# 构建所有包
pnpm build

# 监听模式构建
pnpm build:watch

# 发布所有包
pnpm publish:all

# 代码检查
pnpm lint
```

### CLI 工具使用
```bash
# 初始化 i18n 项目
voerkai18n init

# 提取需要翻译的文本
voerkai18n extract

# 自动翻译（使用 qwen API）
voerkai18n translate --api qwen

# 编译语言包
voerkai18n compile

# 生成 TypeScript 支持
voerkai18n compile --typescript

# 指定模块类型
voerkai18n compile --module-type esm,cjs
```

### 测试
```bash
# 运行运行时测试
pnpm test:runtime

# 运行单个包的测试（在 packages 目录下）
cd packages/runtime && pnpm test
cd packages/runtime && pnpm test:coverage
```

### 文档
```bash
#
```

</details>
