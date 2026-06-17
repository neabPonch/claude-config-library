---
name: KLR-Pattern__fastapi-voyager
source: https://github.com/KLR-Pattern/fastapi-voyager/blob/7db1a94cfae51a5df71690a2a6cecbb1340e4189/CLAUDE.md
repo: KLR-Pattern/fastapi-voyager
kind: claude-md
stars: 446
last_pushed: 2026-05-12T13:09:32Z
license: mit
score: 8
domains: [web-frontend, backend-api, fullstack]
tags: [vite, vue3, fastapi, build-automation]
curated: 2026-06-14
curated_by: config-scout
---

# KLR-Pattern/fastapi-voyager — claude-md

**Why it's worth keeping:** Excellent use of a 'Key Files' map and explicit documentation of the custom template-replacement mechanism used to inject variables into the production build.

**Summary:** Provides detailed build and development instructions for a Python package containing a nested Vue 3 frontend.

**Source credibility:** High; well-starred, recently updated, and uses modern toolchains like uv and Vite.

**Recency:** Very current, utilizing modern Python dependency management (uv) and Node.js patterns.

**Source:** [KLR-Pattern/fastapi-voyager/CLAUDE.md](https://github.com/KLR-Pattern/fastapi-voyager/blob/7db1a94cfae51a5df71690a2a6cecbb1340e4189/CLAUDE.md) · 446★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - fastapi-voyager

## 项目概述

FastAPI Voyager 是一个 Python 包，提供 API 路由树和依赖关系的可视化。前端使用 Vue 3 + Naive UI，通过 Vite 构建。

## 前端构建

前端源码位于 `src/fastapi_voyager/web/`，构建产物为 `src/fastapi_voyager/web/dist/`。

```bash
# 安装依赖（首次或 package.json 变更后）
. "$HOME/.nvm/nvm.sh" && nvm use 20
npm --prefix src/fastapi_voyager/web install

# 构建（修改前端代码后执行）
npm --prefix src/fastapi_voyager/web run build
```

构建产物 `dist/` 已在 `.gitignore` 中，通过 `pyproject.toml` 的 `force-include` 在 CI 打包时包含。

## 开发模式

```bash
# 终端 1：启动 Python 后端（任选一个 demo app）
uv run uvicorn demo_app:app --port 8000
# 或
. .venv/bin/activate && uvicorn demo_app:app --port 8000

# 终端 2（可选）：Vite dev server，支持 HMR
cd src/fastapi_voyager/web && npm run dev
# 浏览器打开 http://localhost:5173，API 请求自动代理到 localhost:8000
```

不启动 Vite dev server 时，直接访问 http://localhost:8000/voyager/ 即可使用构建后的版本。

## 关键文件

| 路径 | 说明 |
|------|------|
| `src/fastapi_voyager/web/src/App.vue` | 主组件（Naive UI） |
| `src/fastapi_voyager/web/src/store.js` | 前端状态管理 |
| `src/fastapi_voyager/web/src/main.js` | Vue 入口 |
| `src/fastapi_voyager/web/src/component/*.vue` | 子组件 |
| `src/fastapi_voyager/web/src/graph-ui.js` | D3 Graphviz 渲染 |
| `src/fastapi_voyager/web/src/magnifying-gl
```

</details>
