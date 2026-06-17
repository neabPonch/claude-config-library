---
name: Fenng__Tech-Doc-Style-Chinese
source: https://github.com/Fenng/Tech-Doc-Style-Chinese/blob/a569c77fcf43e90222676e39f0ef6a5db25fdb68/SKILL.md
repo: Fenng/Tech-Doc-Style-Chinese
kind: skill
stars: 360
last_pushed: 2026-04-16T17:50:37Z
license: mit
score: 9
domains: [technical-writing, documentation, localization]
tags: [style-guide, chinese-language, tech-docs]
curated: 2026-06-15
curated_by: config-scout
---

# Fenng/Tech-Doc-Style-Chinese — skill

**Why it's worth keeping:** Provides extremely specific 'negative constraints' (blacklisted buzzwords) and mapping tables for technical status terms that prevent generic AI translation styles. The inclusion of mechanical rules like case normalization and spacing makes it a perfect high-precision instruction set for an agent.

**Summary:** A highly specialized style guide for writing professional, restrained, and scanable Chinese technical documentation. It covers tone regulation, punctuation standards, CJK-ASCII spacing, and semantic terminology normalization.

**Source credibility:** Strong; 360 stars and active maintenance in the Chinese developer community.

**Recency:** Current and highly practical for modern technical documentation workflows.

**Source:** [Fenng/Tech-Doc-Style-Chinese/SKILL.md](https://github.com/Fenng/Tech-Doc-Style-Chinese/blob/a569c77fcf43e90222676e39f0ef6a5db25fdb68/SKILL.md) · 360★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tech-doc-style-chinese
description: 在撰写、改写或审阅中文技术文档、文档首页、产品文案、界面文案、Markdown 文档或接口说明时使用。采用克制、准确、可扫读的中文技术写作风格：避免第二人称和宣传腔，统一使用直角引号，在可见正文中处理中文与英文或数字的留白，不改动代码字面量、JSON 键名、URL、API 路径等机器可读内容。如项目存在专属术语、版本展示或信息架构约定，再按需读取 references/Project-Overrides.md。
---

# 中文技术文档与产品文案排版规范

<!-- 作者：Fenng（GitHub：@Fenng） -->

在以下任务中使用这份 Skill：

- 文档首页、落地页、首屏文案
- 接口文档、参数说明、常见问题、更新日志
- 产品能力介绍、解决方案页、能力说明页
- 界面文案、按钮文案、导航标签、提示信息

不要用这份 Skill 去改写代码字面量、JSON 键名、URL、API 路径、数据库字段名或其他机器可读标识符。

如果项目存在专属术语、版本展示、信息架构或品牌约定，再按需读取 `references/Project-Overrides.md`。

## 目标

- 准确先于修辞
- 清晰先于热闹
- 导航感先于宣传感
- 可扫读先于堆砌解释
- 以信息架构和内容组织引导阅读，而不是依赖修辞或口号式表达

## 语气

- 使用克制、直接、可执行的中文
- 以说明、界定、引导为主，不用夸张宣传语
- 避免「领先」「强大」「重磅」「颠覆」「震惊」「炸裂」「恭喜」等空泛形容
- 优先陈述「是什么、适用于什么、下一步看哪里」
- 不用第二人称
- 避免问候式开场、平台营销话术和口号式抽象表达
- 避免使用 `Hello`、`Hi` 这类问候式开场

### 黑话短名单

默认避免以下高危黑话词，除非用户明确要求保留，或该词在当前语境中有严格业务定义：

- `赋能`
- `抓手`
- `闭环`
- `沉淀`
- `对齐`
- `对标`
- `拉通`
- `打通`
- `协同`
- `联动`
- `洞察`
- `赛道`
- `心智`
- `调性`
- `战役`
- `链路`
- `势能`
- `兜底`

以下中危词只有在语义明确时才使用：

- `场景`
- `生态`
- `体系`
- `路径`
- `触点`
- `卡点`
- `布局`
- `矩阵`
- `颗粒度`
- `复盘`
- `梳理`
- `输出`
- `提炼`

优先替换为更具体的表达：

- `赋能` -> `提供`
- `抓手` -> `关键措施`
- `闭环` -> `完整流程`
- `沉淀` -> `形成` / `积累`
- `对齐` -> `统一`
- `拉通` / `打通` ->
```

</details>
