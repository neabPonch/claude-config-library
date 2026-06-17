---
name: PenglongHuang__chinese-novelist-skill
source: https://github.com/PenglongHuang/chinese-novelist-skill/blob/eb1185649437f2aaaa765f02be024132ea83d82d/SKILL.md
repo: PenglongHuang/chinese-novelist-skill
kind: skill
stars: 2042
last_pushed: 2026-06-04T08:37:30Z
license: unknown
score: 8
domains: [creative-writing, agents-ai, content-automation]
tags: [long-form, state-management, automated-validation, multi-agent]
curated: 2026-06-14
curated_by: config-scout
---

# PenglongHuang/chinese-novelist-skill — skill

**Why it's worth keeping:** It implements a JSON-based 'writing plan' for cross-session state persistence and an automated 'write-check-rewrite' loop that minimizes human intervention during long runs.

**Summary:** A multi-phase agent workflow designed for long-form novel creation using structured state management and automated quality control. It transitions from iterative preference gathering to autonomous chapter generation and self-correction.

**Source credibility:** High; significant social proof with over 2,000 stars.

**Recency:** Current; utilizes advanced agentic patterns like sub-agent parallelism and automated validation loops.

**Source:** [PenglongHuang/chinese-novelist-skill/SKILL.md](https://github.com/PenglongHuang/chinese-novelist-skill/blob/eb1185649437f2aaaa765f02be024132ea83d82d/SKILL.md) · 2042★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chinese-novelist
description: |
  分章节创作引人入胜的中文小说。支持各种题材（悬疑/言情/奇幻/科幻/历史等），支持10-50章长篇创作，每章3000-5000字，结尾设置悬念钩子。强调深度润色去除AI痕迹，确保文字自然流畅。
  当用户要求：写小说、创作故事、分章节写作、连续剧情、章节悬念、长篇小说时使用。
metadata:
  trigger: 创作中文小说、分章节故事、长篇小说创作
  source: 基于小说创作最佳实践设计
---

# Chinese Novelist: 中文小说创作助手

## 三大黄金法则

1. **展示而非讲述** - 用动作和对话表现，不要直接陈述
2. **冲突驱动剧情** - 每章必须有冲突或转折
3. **悬念承上启下** - 每章结尾必须留下钩子

## 特性说明

- **中断续写**：自动检测未完成项目，从断点继续创作
- **自动校验**：创作完成后自动检查字数和质量，不合格自动修复
- **并行写作**（可选）：支持子Agent并行写作，通过 `02-写作计划.json` 协调状态

## 核心流程

进入每个阶段时，先阅读对应的流程文档以获取详细执行指令。

### 第0步：初始化与偏好加载

读取用户偏好，检测未完成项目（中断续写），展示个性化欢迎。 → 详见 [phase0-initialization.md](references/flows/phase0-initialization.md)

### 第一阶段：三层递进式问答

通过递进式问答收集创作需求，确定小说定位与标题：

- **核心定位**（必答，Q1-Q3）：题材创意、主角设定、核心冲突 → 详见 [phase1-layer1-core.md](references/flows/phase1-layer1-core.md)
- **深度定制与规格**（Q4-Q8）：世界观、视角基调、核心主题、读者定位、章节数量、配置确认 → 详见 [phase1-layer2-customize.md](references/flows/phase1-layer2-customize.md)
- **标题生成**：AI 基于创意元素生成候选标题，用户选择或自定义 → 详见 [phase1-layer3-title.md](references/flows/phase1-layer3-title.md)

### 第二阶段：规划 + 二次确认

创建项目文件夹（`./chinese-novelist/{timestamp}-{小说名称}/`），生成大纲、人物档案和写作计划JSON，等待用户确认。 → 详见 [phase2-planning.md](references/flows/phase2-
```

</details>
