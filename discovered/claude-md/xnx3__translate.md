---
name: xnx3__translate
source: https://github.com/xnx3/translate/blob/229829395b23e3fa5ea478e64508a8d67736aa1f/CLAUDE.md
repo: xnx3/translate
kind: claude-md
stars: 3003
last_pushed: 2026-06-12T07:18:34Z
license: mit
score: 9
domains: [web-frontend, i18n]
tags: [javascript, architecture-guidance, configuration-schema]
curated: 2026-06-16
curated_by: config-scout
---

# xnx3/translate — claude-md

**Why it's worth keeping:** It explicitly identifies boundaries where the AI should avoid manual edits (AUTO_VERSION blocks) and explains the schema of the configuration object to prevent API misuse.

**Summary:** Provides high-context architecture mapping and crucial 'do not touch' warnings for automated versioning blocks.

**Source credibility:** Highly credible: 3000+ stars and actively maintained within the last month.

**Recency:** Very current, mentioning React 19 and modern build tools like Vite.

**Source:** [xnx3/translate/CLAUDE.md](https://github.com/xnx3/translate/blob/229829395b23e3fa5ea478e64508a8d67736aa1f/CLAUDE.md) · 3003★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

**i18n-jsautotranslate** - 一个开源的网页自动翻译解决方案，仅需两行 JS 代码即可实现网页的多语言国际化。

- **NPM 包名**: i18n-jsautotranslate
- **当前版本**: 3.18.98
- **许可证**: MIT
- **作者**: 管雷鸣
- **仓库**: https://github.com/xnx3/translate

## 核心架构

### 主要目录结构

```
translate.js/          # 核心翻译引擎（12433行代码）
  ├── translate.js     # 主入口文件
  ├── translate.min.js # 压缩版本
  ├── debug.js         # 调试工具
  └── demo*.html       # 演示文件

extend/                # 框架扩展和集成
  ├── ArcoDesign/      # ArcoDesign Vue3 集成
  ├── naiveUI/         # NaiveUI 集成
  ├── vant/            # Vant 移动端 UI 集成
  ├── vue/             # Vue3 集成
  ├── react/           # React 集成
  ├── uniapp/          # UniApp 跨平台集成
  ├── chrome_plugin/   # Chrome 浏览器插件
  ├── wordpress/       # WordPress 插件
  ├── translate.core/  # Java 核心库（Maven 项目）
  ├── translate.service-admin/  # 翻译服务管理后台
  └── translate100/    # 轻量级翻译模型

deploy/                # 部署脚本
dev/                   # 开发工具
doc/                   # 文档
```

### 核心翻译引擎 (translate.js)

核心文件位于 `translate.js/translate.js`，包含以下主要模块：

- **translate.execute()** - 执行翻译的主方法
- **translate.listener** - 页面
```

</details>
