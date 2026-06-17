---
name: taishan1994__Agent-Handbook__auto-skill
source: https://github.com/taishan1994/Agent-Handbook/blob/9f8efb782c82e2f8d72e42f92a240b093b58d7f1/skills/auto_skill.md
repo: taishan1994/Agent-Handbook
kind: skill
stars: 26
last_pushed: 2026-04-28T02:14:11Z
license: mit
score: 8
domains: [agents-ai, llm-orchestration]
tags: [skill-schema, agent-framework, lifelong-learning]
curated: 2026-06-16
curated_by: config-scout
---

# taishan1994/Agent-Handbook — skill

**Why it's worth keeping:** The proposed tuple structure—incorporating specific triggers, examples, and versioning—is a superior template compared to standard flat prompts.

**Summary:** Provides a sophisticated blueprint for structured 'SKILL.md' files, including mechanisms for triggers and version control.

**Source credibility:** High-quality academic framework from East China Normal University & Shanghai AI Lab.

**Recency:** Extremely cutting-edge/future-dated (2026) approach to agentic skill evolution.

**Source:** [taishan1994/Agent-Handbook/skills/auto_skill.md](https://github.com/taishan1994/Agent-Handbook/blob/9f8efb782c82e2f8d72e42f92a240b093b58d7f1/skills/auto_skill.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AutoSkill：基于经验驱动的终身学习框架

## 论文概述

**标题**：AutoSkill: Experience-Driven Lifelong Learning via Skill Self-Evolution  
**作者**：Yutao Yang, Junsong Li, Qianjun Pan 等（华东师范大学 & 上海人工智能实验室）  
**发布时间**：2026年3月（arXiv:2603.01145v2）

## 研究背景与动机

在实际的大语言模型（LLM）应用中，用户经常重复表达稳定的偏好和需求，例如：
- 减少幻觉
- 遵循机构写作规范
- 避免过于技术化的措辞
- 遵守特定的工作流程

然而，这些交互经验很少被整合为可重用的知识，导致LLM代理无法在不同会话中积累个性化能力。现有的解决方案存在局限：
- **参数更新方法**：成本高且难以控制
- **基于记忆的方法**：仅存储文本片段而非可操作的行为
- **技能学习方法**：技能通常隐含在提示或策略中，缺乏显式管理

## AutoSkill核心创新

AutoSkill是一个**经验驱动的终身学习框架**，使LLM代理能够：
1. **自动提取**：从对话和交互痕迹中推导技能
2. **持续维护**：支持技能的自我进化
3. **动态重用**：在不重新训练基础模型的情况下，将相关技能注入未来请求

### 关键特性

- **模型无关的插件层**：兼容现有LLM
- **标准化技能表示**：支持跨代理、用户和任务的技能共享与迁移
- **显式技能工件**：将短暂交互经验转化为明确、可重用、可组合的能力
- **完整技能生命周期**：涵盖提取、表示、精炼、检索和重用

## 技术架构

### 双循环设计

1. **技能增强响应生成**（前台路径）
   - 查询重写 → 混合技能检索 → 技能条件生成

2. **技能实时进化**（后台路径）
   - 技能提取 → 检索辅助管理 → 版本化合并

### 技能表示格式

每个技能表示为结构化元组：
```
s = (name, description, prompt, triggers, tags, examples, version)
```

技能以`SKILL.md`文件形式存储，包含：
- 目标与约束
- 工作流（可选）
- 触发条件
- 示例
- 版本号

### 核心模块

1. **查询重写模块**：将当前查询转换为独立的检索查询
2. **混合检索机制**：结合稠密语义匹配（向量相似度）和 lexical 匹配（BM25）
3. **技能提取模块**：仅从用户查询中提取可重用模式
4. **技能管理决策**：决定添加、合并或丢弃候选技能
5. **版本化合并**：迭代优化现有技能而非创建重复项
```

</details>
