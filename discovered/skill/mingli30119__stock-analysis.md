---
name: mingli30119__stock-analysis
source: https://github.com/mingli30119/stock-analysis/blob/7ca91c5b8ac0203af307c67ad5151aad9fb9e6df/SKILL.md
repo: mingli30119/stock-analysis
kind: skill
stars: 535
last_pushed: 2026-05-30T15:00:30Z
license: mit
score: 9
domains: [finance, agents-ai, data-visualization]
tags: [stock-analysis, html-generation, automation]
curated: 2026-06-15
curated_by: config-scout
---

# mingli30119/stock-analysis — skill

**Why it's worth keeping:** The 'Batch-Write + Grep-Verify' protocol is a masterclass in ensuring large file integrity; it uses mechanical validation to prevent truncation or syntax errors. It also provides excellent instructions for injecting complex technical data into JS templates.

**Summary:** A sophisticated multi-phase workflow that automates end-to-end stock research and generates high-fidelity interactive HTML reports.

**Source credibility:** Highly credible with 535 stars and very recent maintenance.

**Recency:** Extremely current, specifically designed for modern agentic tool-use patterns like incremental updates and self-correction via grep.

**Source:** [mingli30119/stock-analysis/SKILL.md](https://github.com/mingli30119/stock-analysis/blob/7ca91c5b8ac0203af307c67ad5151aad9fb9e6df/SKILL.md) · 535★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: stock-analysis-enhanced
description: 一句话搞定个股分析 — 说"分析XXX"，自动采集30+数据源 → AI完成基本面(Step 0-8)+技术面+资金面的完整研报 → 生成交互式HTML报告。支持增量更新（K线/行情/技术指标自动刷新）。触发词："分析XXX股票"（首次）或"更新XXX股票"（增量）。
trigger_keywords: ["分析股票", "个股分析", "股票研究", "分析一只股票", "更新股票", "刷新报告", "增量更新"]
version: 3.1
last_updated: 2026-05-30
variant: enhanced
---

# 一句话搞定个股分析

> 版本：v3.1 | 更新：2026-05-30 | 用户说一句话 → 30+数据源采集 → Step 0-8 基本面 + 第9章技术面 + 资金面 → 双主题交互式HTML

---

## 📋 快速导航

- [⚡ 使用方式](#使用方式) — 一句话触发，全自动执行
  - [场景判断](#场景判断)
  - [场景A：首次分析](#场景a首次分析) — 完整三阶段
  - [场景B：增量更新](#场景b增量更新) — 快速刷新数据
- [🏗️ 三层架构](#三层架构) — Phase 1 数据采集 → Phase 2 AI分析 → Phase 3 HTML
- [📊 输出内容](#输出内容) — MD 报告 + HTML 报告的完整结构
- [🎨 HTML手写规范](#html手写规范) — 分批手写 + grep 机械校验
- [🔧 执行流程](#执行流程) — Phase 1/2/3 详细步骤
- [🔄 增量更新详细说明](#增量更新详细说明) — 脚本自动 + AI 手动

---

## ⚡ 使用方式

### 场景判断

**AI必须根据用户输入的关键词判断场景：**

#### 场景A：首次分析（完整流程）

**触发关键词：**
- "分析 XXX股票"
- "个股分析 XXX"
- "研究 XXX"
- "生成 XXX报告"
- 用户明确说"首次分析"

**判断逻辑：**
- 用户输入包含上述关键词 → 执行首次分析（Phase 1→2→3）

#### 场景B：增量更新（只更新数据）

**触发关键词：**
- "更新 XXX股票"
- "刷新 XXX报告"
- "增量更新 XXX"
- "更新报告"
- 用户明确说"更新"

**判断逻辑：**
1. 用户输入包含上述关键词
2. 检查 `output/个股研究-{股票名称}.html` 是否存在
3. 如果存在 → 执行增量更新
4. 如果不存在 → 提示用户："未找到 XXX 的报告，是否需要首次分析？"

---

#
```

</details>
