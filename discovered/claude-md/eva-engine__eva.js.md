---
name: eva-engine__eva.js
source: https://github.com/eva-engine/eva.js/blob/0038f1bd1da5bef13cd121daac3eafeb2feab166/CLAUDE.md
repo: eva-engine/eva.js
kind: claude-md
stars: 1780
last_pushed: 2026-06-15T06:27:20Z
license: mit
score: 9
domains: [game-engine, frontend, monorepo]
tags: [typescript, ecs, pixijs, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# eva-engine/eva.js — claude-md

**Why it's worth keeping:** It explicitly defines the ECS architecture pattern and critical package dependency chains that prevent build errors, while also documenting specific CLI flags and TypeScript path aliases.

**Summary:** Provides a comprehensive structural and architectural guide for a monorepo-based game engine.

**Source credibility:** High; the project has significant community validation (1780 stars) and active maintenance.

**Recency:** Current; uses modern Monorepo patterns (npm workspaces/Lerna) and TypeScript configurations.

**Source:** [eva-engine/eva.js/CLAUDE.md](https://github.com/eva-engine/eva.js/blob/0038f1bd1da5bef13cd121daac3eafeb2feab166/CLAUDE.md) · 1780★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Eva.js

Eva.js 是一个基于 ECS（Entity-Component-System）架构的前端互动游戏引擎，底层渲染基于 PixiJS。

## 项目结构

Monorepo（Lerna + npm workspaces），所有包位于 `packages/` 目录下，包名以 `@eva/` 为前缀。

### 参考源码

`temp/hd-pixijs/` 目录包含 PixiJS 源码，仅作为阅读参考，用于理解 Eva.js 底层渲染能力。**不要修改该目录下的任何文件。**

## Packages 说明

### 核心

| 包 | 说明 |
|---|---|
| `@eva/eva.js` | 核心引擎，提供 Game、GameObject、Component、System、Transform、Scene、资源加载器、装饰器、游戏循环 |
| `@eva/plugin-renderer` | 核心渲染系统，初始化 PixiJS Application/Canvas，提供 RendererSystem |
| `@eva/renderer-adapter` | 渲染器抽象层，将 PixiJS 显示对象封装为统一适配器 API |

### 渲染插件

| 包 | 说明 |
|---|---|
| `@eva/plugin-renderer-img` | 图片渲染（IMAGE 资源类型） |
| `@eva/plugin-renderer-sprite` | 精灵图渲染（Sprite Atlas） |
| `@eva/plugin-renderer-sprite-animation` | 帧动画播放 |
| `@eva/plugin-renderer-text` | 文本渲染（Text / HTMLText / BitmapText 三种模式） |
| `@eva/plugin-renderer-graphics` | 矢量图形绘制（矩形、圆形、线条等） |
| `@eva/plugin-renderer-nine-patch` | 九宫格缩放（UI 面板/按钮常用） |
| `@eva/plugin-renderer-tiling-sprite` | 平铺精灵（滚动背景等） |
| `@eva/plugin-renderer-mask` | 遮罩/裁剪（形状遮罩或图片 Alpha 遮罩） |
| `@eva/plugin-renderer-mesh` | 透视网格变形（四角顶点变换） |
| `@eva/plugin-renderer-render` | 渲染属性控制（alpha、visible、zIndex、sortableChildren） |
| `@eva/plugin-renderer-event` | 触摸/指针事件系统（
```

</details>
