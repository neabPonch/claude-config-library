---
name: wxingheng__markdown-to-image-serve
source: https://github.com/wxingheng/markdown-to-image-serve/blob/05092cbd50e11e1edde246f5d7730a6b38b72687/CLAUDE.md
repo: wxingheng/markdown-to-image-serve
kind: claude-md
stars: 269
last_pushed: 2026-03-01T12:02:02Z
license: mit
score: 8
domains: [web-frontend, backend-api, devops]
tags: [nextjs, puppeteer, documentation-rich]
curated: 2026-06-15
curated_by: config-scout
---

# wxingheng/markdown-to-image-serve — claude-md

**Why it's worth keeping:** Includes critical 'tribal knowledge' such as the patch-package requirement, mixed router patterns (App vs Pages), and specific environment variables needed for headless browser operation.

**Summary:** A highly detailed technical manual that covers architecture, API specifications, and deployment workflows. It provides essential context for complex system interactions like Puppeteer/Chrome integration.

**Source credibility:** Solid; 269 stars indicates a useful utility with well-maintained documentation.

**Recency:** Very current; utilizes modern tech stacks like Next.js 14 and React 18.

**Source:** [wxingheng/markdown-to-image-serve/CLAUDE.md](https://github.com/wxingheng/markdown-to-image-serve/blob/05092cbd50e11e1edde246f5d7730a6b38b72687/CLAUDE.md) · 269★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Markdown to Image Serve - Claude AI 开发指南

## 项目概述

这是一个基于 Next.js 的 Markdown 转图片服务，提供 Web 编辑器和 RESTful API。用户可以输入 Markdown 内容，系统会生成精美的海报图片。

**核心价值**: 将 Markdown 内容转换为可在社交媒体分享的精美图片

**主要功能**:
- Markdown 实时预览编辑器
- 9 种内置主题 (blue, pink, purple, green, yellow, gray, red, indigo, SpringGradientWave)
- 自定义页眉、页脚、Logo
- 中文字体支持 (SimSun)
- RESTful API 接口
- Docker 容器化部署

## 技术栈

| 类别 | 技术 |
|------|------|
| 框架 | Next.js 14.2.3 (App Router + Pages Router 混合模式) |
| 语言 | TypeScript 5 |
| UI | React 18 + Tailwind CSS 3.4 + Radix UI + shadcn/ui |
| 图表生成 | Puppeteer Core + @sparticuz/chromium-min |
| Markdown | markdown-to-poster 0.0.9 + @uiw/react-md-editor |
| 部署 | Docker + Railway/Render/Fly.io 支持 |

## 项目结构

```
src/
├── app/                    # Next.js App Router
│   ├── page.tsx           # 首页 - Markdown 编辑器
│   ├── docs/page.tsx      # 文档页面
│   ├── layout.tsx         # 根布局 (Header + Footer)
│   └── globals.css        # 全局样式
│
├── pages/                  # Next.js Pages Router (API)
│   ├── api/
│   │   ├── generatePoster.ts       # 返回图片 Buffer
│   │   ├── generatePosterImage.ts  # 返回图片 URL
│   │   └── images/[filename].ts    # 图片服务端点
│   └── poster/index.tsx            # 海报渲染页面
│
├── com
```

</details>
