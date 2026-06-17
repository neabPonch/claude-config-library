---
name: yhslgg-arch__url-reader
source: https://github.com/yhslgg-arch/url-reader/blob/2ff3edbd742a89b2d57c818057c65c7912668b44/skill.md
repo: yhslgg-arch/url-reader
kind: skill
stars: 180
last_pushed: 2026-02-05T16:28:24Z
license: unknown
score: 9
domains: [web-scraping, automation, data-extraction]
tags: [scraper, archiving, fallback-logic]
curated: 2026-06-16
curated_by: config-scout
---

# yhslgg-arch/url-reader — skill

**Why it's worth keeping:** The hierarchical failure recovery mechanism is a perfect pattern for agentic reliability. The specific implementation of local file organization, including automated image downloading and dated directories, makes it an end-to-end archiving tool rather than just a scraper.

**Summary:** A high-reliability web scraping tool that implements a three-layer fallback strategy (API/AI → API → Playwright) to extract and archive content into Markdown.

**Source credibility:** Solid; 180 stars suggests high real-world utility for the target demographic.

**Recency:** Current; utilizes modern scraping libraries like Firecrawl and Playwright compatible with agentic workflows.

**Source:** [yhslgg-arch/url-reader/skill.md](https://github.com/yhslgg-arch/url-reader/blob/2ff3edbd742a89b2d57c818057c65c7912668b44/skill.md) · 180★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: url-reader
description: 智能读取任意URL内容，支持微信公众号、小红书、今日头条、抖音、淘宝、天猫、京东、百度等中国主流平台，自动识别平台类型并提取核心内容。自动保存内容为Markdown，下载图片到本地。
---

# URL Reader - 智能网页内容读取器

一键读取任意URL的内容，自动识别平台类型，智能选择最佳读取策略，**自动保存内容和图片到本地**。

## 默认保存目录

```
/Users/ys/laoyang知识库/nickys/素材/
```

保存格式：
```
素材/
└── 2026-01-30_文章标题/
    ├── content.md      # Markdown内容
    ├── img_01.webp     # 图片1
    ├── img_02.webp     # 图片2
    └── ...
```

## 核心技术方案

### 三层读取策略（自动降级）

```
┌─────────────────────────────────────────────────────────────────┐
│                     URL Reader 技术架构                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  用户输入 URL                                                    │
│       ↓                                                         │
│  ┌─────────────┐                                                │
│  │ 平台识别器   │ → 识别URL所属平台（微信/小红书/淘宝等）           │
│  └─────────────┘                                                │
│       ↓                                                         │
│  ┌─────────────────────────────────────────────────────────────┐│
│  │                    策略选择器
```

</details>
