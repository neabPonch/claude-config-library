---
name: FlameskyDexive__Legends-Of-Heroes__skill
source: https://github.com/FlameskyDexive/Legends-Of-Heroes/blob/a0b6258b5de64e2d56e6136bfa2b3d84fbc923a7/.codex/skills/unity-yaml-editing/SKILL.md
repo: FlameskyDexive/Legends-Of-Heroes
kind: skill
stars: 898
last_pushed: 2026-06-12T00:25:01Z
license: other
score: 8
domains: [game-dev, unity]
tags: [unity, yaml, serialization, asset-pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# FlameskyDexive/Legends-Of-Heroes — skill

**Why it's worth keeping:** The 'Decision Order' logic and strict constraints on GUID/fileID preservation provide an excellent template for interacting with any fragile, highly-structured serialization format.

**Summary:** Provides a specialized fallback workflow for direct text-based manipulation of Unity's sensitive YAML serialized assets when high-level APIs are insufficient.

**Source credibility:** High; derived from a well-starred game framework repository.

**Recency:** Current; tailored for modern Unity/C# development workflows.

**Source:** [FlameskyDexive/Legends-Of-Heroes/.codex/skills/unity-yaml-editing/SKILL.md](https://github.com/FlameskyDexive/Legends-Of-Heroes/blob/a0b6258b5de64e2d56e6136bfa2b3d84fbc923a7/.codex/skills/unity-yaml-editing/SKILL.md) · 898★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unity-yaml-editing
description: Unity YAML text serialization editing workflow. Use when Codex needs to directly inspect, modify, create, or repair Unity serialized YAML files such as .unity scenes, .prefab assets, .asset ScriptableObject/config files, .mat, .controller, or other text-serialized Unity assets, especially when AIBridge inspector/prefab/scene APIs do not support the requested Prefab, Scene, ScriptableObjectTable, or custom asset operation.
---

# Unity YAML Editing

Use this Skill only after considering Unity/AIBridge APIs. UnityYAML is fragile; direct text edits are the fallback for unsupported serialized asset operations, deterministic repair work, and rare text-serialized asset authoring that AIBridge/Unity APIs cannot express.

## Decision Order

1. Prefer `aibridge` Inspector/SerializedProperty commands for single readable field edits on scene objects, prefab assets, and `.asset` files.
2. Prefer `inspector set_properties` for small batched field edits on one target.
3. Prefer `aibridge-prefab-patch` for complex Prefab child/component/property/array/reference edits it supports.
4. Prefer Unity Editor scripts when generating high-level assets that Unity
```

</details>
