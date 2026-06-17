---
name: huangruiteng__CS-Notes__skill
source: https://github.com/huangruiteng/CS-Notes/blob/6914c87fcb5774a4e2f2f94c0917df5e643a8dc0/.trae/openclaw-skills/common-fetcher/SKILL.md
repo: huangruiteng/CS-Notes
kind: skill
stars: 3946
last_pushed: 2026-06-11T10:05:19Z
license: mit
score: 8
domains: [data-scraping, cli-tools, agents-ai]
tags: [scraper, industry-data, structured-metadata]
curated: 2026-06-16
curated_by: config-scout
---

# huangruiteng/CS-Notes — skill

**Why it's worth keeping:** Provides an excellent template for tool definition including dependency management, installation steps, and clear CLI command structures. The inclusion of performance benchmarks is a high-level technique to help agents assess tool reliability.

**Summary:** A unified data collection framework providing industry-specific scraping via a CLI and Node.js API. It includes structured metadata designed for seamless agent integration.

**Source credibility:** High-star repository (3.9k) indicating a reliable/active developer source.

**Recency:** Extremely current, with activity within the last month.

**Source:** [huangruiteng/CS-Notes/.trae/openclaw-skills/common-fetcher/SKILL.md](https://github.com/huangruiteng/CS-Notes/blob/6914c87fcb5774a4e2f2f94c0917df5e643a8dc0/.trae/openclaw-skills/common-fetcher/SKILL.md) · 3946★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: common-fetcher
version: 1.0.0
description: 统一采集框架 - 支持 RSS/Web/API，207+ 采集源，AI 评分/分类/摘要
metadata: {
  "openclaw": {
    "emoji": "🕸️",
    "category": "data",
    "requires": {
      "bins": ["node", "npm"],
      "env": [],
      "config": []
    },
    "primaryEnv": "",
    "install": [
      {
        "id": "npm-install",
        "kind": "node",
        "package": "common-fetcher",
        "bins": ["common-fetcher"],
        "label": "Install common-fetcher (npm)"
      }
    ]
  }
}
---

# Common-Fetcher

统一采集框架，为 AI Agent 提供强大的信息采集能力。

## 功能特性

- 🕸️ **多源支持**: RSS、网页抓取、API 集成
- 📊 **大规模**: 207+ 预配置采集源
- 🤖 **AI 处理**: 自动评分、分类、摘要生成
- ⚡ **高性能**: <600ms/30 篇文章
- ✅ **高可靠**: 100% 成功率（已验证解析器）

## 支持的行业

### 🏭 煤炭行业（27 个采集源）
- 国家级：发改委、能源局等 6 个
- 省级：4 个
- 市级：3 个
- 数据平台：4 个
- 企业自媒体：10 个

### 🏠 房地产行业（23 个采集源）
- 国家级：住建部、央行等 5 个
- 省级：1 个
- 市级：3 个
- 数据平台：4 个
- 企业自媒体：10 个

### 🤖 AI 技术（129 个采集源）
- RSS 源：90 个（Hacker News, MIT Tech Review 等）
- 网站/自媒体：39 个

## 使用方法

### CLI 方式

```bash
# 抓取煤炭行业数据
common-fetcher --industry coal --output daily.md

# 抓取房地产行业数据
common-fetcher --industry realestate --output daily.md

# 抓取 AI 技术数据
common-fetcher --industry ai --output daily.md

# 自定义采集源
common-f
```

</details>
