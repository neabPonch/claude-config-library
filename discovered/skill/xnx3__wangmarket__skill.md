---
name: xnx3__wangmarket__skill
source: https://github.com/xnx3/wangmarket/blob/27fb477487f94224f1f7b6622e1babef843438b8/skills/wangmarket-dev/SKILL.md
repo: xnx3/wangmarket
kind: skill
stars: 343
last_pushed: 2026-04-04T12:58:23Z
license: other
score: 8
domains: [web-development, backend-systems]
tags: [architecture-rules, workflow-optimization, context-injection]
curated: 2026-06-15
curated_by: config-scout
---

# xnx3/wangmarket — skill

**Why it's worth keeping:** It teaches a high-level 'upgrade-safe' priority (Plugins > Overwrites > Core) and mandates a documentation-first discovery workflow before any code changes occur.

**Summary:** A specialized developer skill for the Wangmarket system that establishes architectural boundaries and specific modification hierarchies.

**Source credibility:** The repository has significant social proof with 343 stars and active maintenance.

**Recency:** Very current, referencing modern tools like `rg` and specific developer workflows suitable for today's agents.

**Source:** [xnx3/wangmarket/skills/wangmarket-dev/SKILL.md](https://github.com/xnx3/wangmarket/blob/27fb477487f94224f1f7b6622e1babef843438b8/skills/wangmarket-dev/SKILL.md) · 343★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: wangmarket-dev
description: 在 wangmarket/网市场 仓库或保持同样目录结构的派生项目中进行安装、运行、模板开发、插件开发、JSP/Spring Boot 二次开发、控制器或视图重写、问题排查与验证时使用。适用于把整个 skills/ 目录直接放到项目根目录后，让大模型自动参考本地仓库结构、官方文档索引与改动工作流；不包含 AI-SEO 产品文档。
---

# Wangmarket Dev

当任务发生在 `wangmarket` 仓库本体，或发生在与本仓库目录结构基本一致的派生项目中时，使用这个 skill。

## 适用范围

- 目标仓库保留了 `src/main/java/com/xnx3/wangmarket/...`、`src/main/webapp/WEB-INF/view/...`、`src/main/resources/application.properties` 这套主体结构。
- 任务涉及安装部署、模板制作、栏目/内容管理、域名访问链路、插件扩展、输入模型、多语种、分布式存储或常规二次开发。
- 这个 skill 只覆盖网市场本体，不覆盖 `AI-SEO` 产品及其安装、配置、SEO 页面。

## 先读哪些文件

1. 先读 `references/repo-architecture.md`，确认当前仓库是不是网市场本体，关键控制器、JSP、插件目录分别在哪。
2. 再读 `references/change-workflows.md`，按任务类型选择推荐落点与验证方式。
3. 当需求依赖官方行为说明、模板机制或扩展优先级时，再读 `references/official-docs.md`。

## 工作原则

- 优先级遵循官方二次开发前言：`功能插件 > 重写指定文件 > 直接修改 wangmarket 本身`。
- 开改之前，先定位实际落点；不要只改 JSP 或只改 Controller，忽略另一半链路。
- 模板类任务，优先检查 `TemplateController`、`ColumnController`、`plugin/templateDevelop`、`websiteTemplate` 与相关 JSP。
- 前台访问、域名、上线链路问题，优先检查 `domain/controller/PublicController.java` 与域名相关官方文档。
- 安装、启动、配置类任务，优先检查 `com/Application.java`、`application.properties`、`InstallController_.java`。
- README 或官网里出现的 `plugin/phoneCreateSite/reg.do` 属于另一个仓库的项目，不在当前
```

</details>
