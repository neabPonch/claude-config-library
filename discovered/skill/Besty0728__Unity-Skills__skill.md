---
name: Besty0728__Unity-Skills__skill
source: https://github.com/Besty0728/Unity-Skills/blob/5194fa8f546a44049b07590f565590c25d759aff/SkillsForUnity/unity-skills~/skills/component/SKILL.md
repo: Besty0728/Unity-Skills
kind: skill
stars: 1235
last_pushed: 2026-06-14T09:28:59Z
license: mit
score: 9
domains: [game-development, automation, unity-engine]
tags: [unity, component-management, api-protocol, batching]
curated: 2026-06-15
curated_by: config-scout
---

# Besty0728/Unity-Skills — skill

**Why it's worth keeping:** It utilizes the 'BATCH-FIRST' pattern to optimize API efficiency and includes specific 'DO NOT' sections to proactively mitigate common LLM hallucinations regarding case sensitivity and function existence.

**Summary:** Defines a highly structured protocol for interacting with Unity GameObject components via automated tool calls. It covers property manipulation, batch processing, and object targeting.

**Source credibility:** High credibility; the repository is well-starred (1235) and shows active maintenance.

**Recency:** 

**Source:** [Besty0728/Unity-Skills/SkillsForUnity/unity-skills~/skills/component/SKILL.md](https://github.com/Besty0728/Unity-Skills/blob/5194fa8f546a44049b07590f565590c25d759aff/SkillsForUnity/unity-skills~/skills/component/SKILL.md) · 1235★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unity-component
description: "GameObject component management — add, remove, list, copy, enable/disable components, read/set component properties. Exact signatures via GET /skills/schema."
---

# Unity Component Skills

> **BATCH-FIRST**: Use `*_batch` skills when operating on 2+ objects to reduce API calls from N to 1.

## Operating Mode

- **Approval**：本模块 Mixed —— `component_list` / `component_get_properties` 标 `SkillMode.SemiAuto`，可直接执行；写类 skill (`component_add` / `component_set_property` / `component_set_enabled` / `component_copy` 等) 标 `SkillMode.FullAuto`，需 grant 单次执行返结果。
- **Auto / Bypass**：FullAuto 直接执行。
- **含 NeverInSemi 高危 skill**：`component_remove` / `component_remove_batch`（Operation.Delete）。这些在 Approval/Auto 下返 `MODE_FORBIDDEN`，仅 Bypass 或 Allowlist 命中可调。

**DO NOT** (common hallucinations):
- `component_create` / `component_get` do not exist → use `component_add` (add) and `component_get_properties` (read)
- `component_find` does not exist → use `component_list` to list components on an object
- `componentType` is case-sensitive — `Rigidbody` not `rigidbody`, `BoxCollider` not `boxcollider`
- Custom scripts need exact class name; if namespaced, use `Namespac
```

</details>
