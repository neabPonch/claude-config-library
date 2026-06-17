---
name: openakita__openakita__skill
source: https://github.com/openakita/openakita/blob/1c91aa902713abcabeabe8aa0d1cb23590b1606c/skills/apify-scraper/SKILL.md
repo: openakita/openakita
kind: skill
stars: 1815
last_pushed: 2026-06-16T03:46:27Z
license: agpl-3.0
score: 9
domains: [web-scraping, data-extraction, agents-ai]
tags: [apify, scraper, automation, structured-data]
curated: 2026-06-16
curated_by: config-scout
---

# openakita/openakita — skill

**Why it's worth keeping:** It provides clear decision-making logic for actor selection and a robust asynchronous batching workflow pattern. The inclusion of 'When to Use' cases and specific error troubleshooting makes it highly actionable for an agent.

**Summary:** A highly structured skill file that enables an agent to perform complex web scraping across social media, search engines, and e-commerce using Apify's ecosystem.

**Source credibility:** High; the source repo is well-starred, active, and professionally structured.

**Recency:** Current; utilizes modern Python async patterns and recent API integration strategies.

**Source:** [openakita/openakita/skills/apify-scraper/SKILL.md](https://github.com/openakita/openakita/blob/1c91aa902713abcabeabe8aa0d1cb23590b1606c/skills/apify-scraper/SKILL.md) · 1815★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: openakita/skills@apify-scraper
description: Web data extraction using 55+ Apify Actors for AI-driven scraping. Supports Instagram, Facebook, TikTok, YouTube, Google, and more. Auto-selects best Actor for the task. Structured output in JSON/CSV with rate limiting and ethical scraping guidelines.
license: MIT
metadata:
  author: openakita
  version: "1.0.0"
---

# Apify Scraper — 网页数据抓取

## When to Use

- 用户需要从网站抓取结构化数据（商品信息、社交媒体帖子、搜索结果等）
- 需要批量获取社交媒体平台数据（Instagram、TikTok、YouTube 等）
- 需要抓取 Google 搜索结果、地图信息、评价数据
- 需要定期监控网页变化
- 需要将非结构化网页内容转换为 JSON/CSV
- 需要从电商平台提取商品和价格信息

---

## Prerequisites

### 必需配置

| 配置项 | 说明 |
|--------|------|
| `APIFY_TOKEN` | Apify API Token，在 https://console.apify.com/account/integrations 获取 |

将 Token 添加到 `.env` 文件：

```
APIFY_TOKEN=apify_api_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

### 必需依赖

| 依赖 | 用途 | 安装方式 |
|------|------|---------|
| `httpx` | HTTP API 调用 | `pip install httpx` |

### 可选依赖

| 依赖 | 用途 | 安装方式 |
|------|------|---------|
| `apify-client` | Apify Python SDK | `pip install apify-client` |
| `pandas` | 数据处理与导出 | `pip install pandas` |

### 验证配置

```bash
curl -s "https://api.apify.com/v2/user/me?token=$APIFY_TOKEN" | python -m json.tool
```

</details>
