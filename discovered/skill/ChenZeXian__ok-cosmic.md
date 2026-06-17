---
name: ChenZeXian__ok-cosmic
source: https://github.com/ChenZeXian/ok-cosmic/blob/5c336e055c5577dc56a8c9814def2c5282644d18/SKILL.md
repo: ChenZeXian/ok-cosmic
kind: skill
stars: 9
last_pushed: 2026-03-30T06:47:28Z
license: apache-2.0
score: 9
domains: [enterprise-software, backend-development, erp-systems]
tags: [decision-matrix, domain-specific, agentic-workflow, kingdee-cosmic]
curated: 2026-06-15
curated_by: config-scout
---

# ChenZeXian/ok-cosmic — skill

**Why it's worth keeping:** Uses an elite 'Encapsulation First' routing logic and a multi-layered decision tree (Matrix -> Routing -> Snippets) to prevent low-level API misuse. The integration of a mandatory post-generation linting step is a top-tier agentic workflow.

**Summary:** A highly structured domain-specific skill for Kingdee Cloud Cosmic development that uses a decision matrix to guide the AI through complex SDK hierarchies.

**Source credibility:** A specialized, well-maintained repository for enterprise software development.

**Recency:** Highly current; utilizes advanced multi-file reasoning patterns optimal for modern Claude Code agents.

**Source:** [ChenZeXian/ok-cosmic/SKILL.md](https://github.com/ChenZeXian/ok-cosmic/blob/5c336e055c5577dc56a8c9814def2c5282644d18/SKILL.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "ok-cosmic"
description: "金蝶云苍穹开发主 Skill，优先复用 kd-cd-cosmic-commons 封装。适用于插件开发、单据/列表/表单逻辑、操作服务、BOTP 转换、后台视图打开、附件处理、DynamicObject 与元数据处理、弹性域解析及 OpenAPI 集成。默认优先使用仓库封装；在涉及原生插件事件、SDK API、方法签名或封装未覆盖场景时，使用内置脚本进行查询。"
---

# 苍穹开发

默认按"封装优先，原生兜底"工作，避免在仓库已封装的场景里退回到 BOS 原生低层 API。

## 最短决策路径

1. 先判断插件类型或能力类别（查下方决策矩阵）。
2. 先读对应 `references/*.md`，确认事件边界与适用场景。
3. 再读对应 `assets/*.java` 模板，沿用已有方法签名和骨架。小场景可直接用 `assets/snippets/*.java`。
4. 字段不确定先查 `cosmic-form-metadata.py`，SDK 签名不确定先查 `cosmic-api-knowledge.py`。
5. 只有"插件类型 + 事件方法 + 字段/签名"都确认后，才开始生成代码。
6. **代码生成后，必须执行 `cosmic-post-lint.py` 自动校验**；若存在 ERROR 级问题须立即修复并重新校验直到通过。

## 快速决策矩阵

| 需求关键词 | 插件类型          | 封装文档 (先读) | 原生文档 (兜底) | 模板文件 |
|---|---------------|---|---|---|
| 表单 UI / 字段联动 / 控件交互 | 表单插件          | [plugin-base.md](references/adv/plugin-base.md) | [plugin-form.md](references/base/plugin/plugin-form.md) | [FormPluginTemplate.java](assets/FormPluginTemplate.java) |
| 单据 UI / 审核提交按钮 | 单据插件          | [plugin-base.md](references/adv/plugin-base.md) | [plugin-bill.md](references/base/plugin/plugin-bill.md) | [BillPlugInTemplate.java](assets/BillPlugInTemplate.java) |
| 列表 / 多选操作 / 批量 | 列表插件          | [plugin-base.md](references/adv/
```

</details>
