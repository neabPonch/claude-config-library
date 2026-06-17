---
name: huangserva__skill-prompt-generator__skill
source: https://github.com/huangserva/skill-prompt-generator/blob/e9512498402f6625300f42b9633d907a28dda126/.codex/skills/prompt-extractor/skill.md
repo: huangserva/skill-prompt-generator
kind: skill
stars: 1387
last_pushed: 2026-05-10T09:16:55Z
license: unknown
score: 9
domains: [agents-ai, prompt-engineering]
tags: [extractor, structured-data, image-generation]
curated: 2026-06-15
curated_by: config-scout
---

# huangserva/skill-prompt-generator — skill

**Why it's worth keeping:** The use of a multi-tier priority system for genre recognition and the 'critical oppositions' logic (required vs forbidden) is an elite pattern for structuring negative constraints.

**Summary:** A sophisticated extraction skill that deconstructs complex AI image prompts into highly granular, structured JSON data including technical specs and facial features.

**Source credibility:** Highly credible with 1.3k+ stars, indicating significant community validation in the AI art space.

**Recency:** Current; utilizes advanced structural decomposition techniques ideal for modern LLM agents.

**Source:** [huangserva/skill-prompt-generator/.codex/skills/prompt-extractor/skill.md](https://github.com/huangserva/skill-prompt-generator/blob/e9512498402f6625300f42b9633d907a28dda126/.codex/skills/prompt-extractor/skill.md) · 1387★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prompt-extractor
description: 自动化提取AI绘画提示词的模块化结构，从海量提示词中提炼可复用的模块组件
---

# Prompt Extractor Skill

自动化提取AI绘画提示词的模块化结构，从海量提示词中提炼可复用的模块组件。

## 核心功能

你是一位提示词工程专家，专注于AI图像生成（如Midjourney、DALL-E、Stable Diffusion）提示词的结构化分析和模块提取。

## 工作流程

当用户调用此skill时，按以下步骤执行：

### 1. 数据读取与预处理

支持两种输入方式：

**方式A：文件路径**
- 接收用户提供的提示词文件路径（支持 txt, csv, json 格式）
- 自动识别文件格式并解析

**方式B：直接粘贴**（推荐用于小批量）
- 用户可以直接粘贴提示词文本（每行一个或用分隔符）
- 无需创建文件，实时处理
- 支持单条或多条（最多100条/次）

**数据清洗：**
- 去重、去除无效短提示（<10字符）
- 统一标点符号
- 如果是CSV/JSON，自动识别包含提示词的列/字段

### 2. 智能聚类分析（仅处理>100条时）

对于大批量数据，先进行主题聚类：
- 基于关键词频率统计（如"微距"、"电影感"、"梦幻"）
- 分组相似提示（建议3-5个主题簇）
- 为每个簇生成主题标签

### 3. 模块化提取

针对每条提示词，提取以下模块：

**核心模块类型（10大类）：**
1. **主体变量** (Subject Variables)：可替换的核心对象（人物、物体、场景）
2. **视觉风格** (Visual Style)：艺术风格、画风、年代感
3. **技术参数** (Technical Parameters)：镜头、光线、分辨率、渲染引擎
4. **细节增强** (Detail Enhancers)：质量修饰词、强调词
5. **情绪氛围** (Mood & Atmosphere)：情感基调、氛围描述
6. **约束条件** (Constraints)：负面提示、排除元素
7. **构图参数** (Composition)：视角、景深、框架比例、对称性、构图法则
8. **色彩方案** (Color Scheme)：色调、配色、饱和度、对比度、色温
9. **时间/季节** (Time & Season)：时间段（黎明/黄昏）、季节、天气状态
10. **参考艺术家/作品** (References)：艺术家引用、特定作品风格、平台风格

### 3.5 特殊模式识别（针对复杂摄影提示词）

**摄影流派自动识别** (10大流派):
扫描关键词自动标记 `photography_genre` 字段，按优先级依
```

</details>
