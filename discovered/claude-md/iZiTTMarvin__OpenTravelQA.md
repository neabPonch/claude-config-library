---
name: iZiTTMarvin__OpenTravelQA
source: https://github.com/iZiTTMarvin/OpenTravelQA/blob/b0cab71f5a544ad4cfb9f04f7cf44763749a6cfc/CLAUDE.md
repo: iZiTTMarvin/OpenTravelQA
kind: claude-md
stars: 5
last_pushed: 2025-12-01T04:48:58Z
license: unknown
score: 9
domains: [agents-ai, data-science, python]
tags: [rag, nlp, architecture-guide]
curated: 2026-06-15
curated_by: config-scout
---

# iZiTTMarvin/OpenTravelQA — claude-md

**Why it's worth keeping:** Excellent use of ASCII flowcharts to explain logic, detailed schema definitions for return types, and specific 'Development Notes' that instruct how to extend the system.

**Summary:** A comprehensive technical manual for a multi-method QA system covering architecture, data schemas, and operational commands.

**Source credibility:** Academic project with 5 stars; provides high-density technical documentation.

**Recency:** 7 months old; highly relevant for modern RAG and agentic workflows.

**Source:** [iZiTTMarvin/OpenTravelQA/CLAUDE.md](https://github.com/iZiTTMarvin/OpenTravelQA/blob/b0cab71f5a544ad4cfb9f04f7cf44763749a6cfc/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个旅游景点智能问答系统，实现了三种不同的问答方法：
1. **基于规则的问答** (Rule-based QA) - 关键词匹配 + 词典实体识别
2. **基于文本分类的问答** (Text Classification QA) - TF-IDF + LinearSVC 意图分类
3. **基于大模型 RAG 的问答** (LLM RAG QA) - 检索增强生成

## 常用命令

### 运行系统
```bash
# 启动 Streamlit Web 应用（主入口）
streamlit run main.py

# 默认会在 http://localhost:8501 启动
```

### 测试单个模块
```bash
# 测试基于规则的问答
python code/rule_based_qa.py

# 测试基于文本分类的问答（会自动训练模型）
python code/text_classification_qa.py

# 测试基于 LLM RAG 的问答
python code/llm_rag_qa.py
```

### 数据预处理
```bash
# 运行数据预处理脚本（如果需要重新处理原始数据）
python data_preprocessing.py

# 修复银川景点名称（特定数据修复脚本）
python fix_yinchuan_names.py
```

### 调试检索功能
```bash
# 调试 RAG 检索功能
python debug_retrieval.py
```

## 核心架构

### 三层问答架构

系统采用**三种独立的问答方法**，每种方法都是完整的端到端实现：

```
用户问题 → [方法选择] → 问答处理 → 生成回答
                ↓
        ┌───────┴────────┐
        │                │
   规则匹配        文本分类        RAG检索
   (关键词)        (机器学习)      (向量+LLM)
```

#### 1. 基于规则的问答 (`code/rule_based_qa.py`)

**核心流程：**
```
用户问题 → 意图识别(关键词匹配) → 实体识别(词典匹配) → 槽位填充 → 模板生成回答
```

**关键组件：**
- `意图关键词映射表`: 12种意图的关键词列表
- `识别意图()`: 基于关键词匹配统计识别意图
```

</details>
