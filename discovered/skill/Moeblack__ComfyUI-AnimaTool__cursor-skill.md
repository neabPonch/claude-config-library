---
name: Moeblack__ComfyUI-AnimaTool__cursor-skill
source: https://github.com/Moeblack/ComfyUI-AnimaTool/blob/2a9c5fcbbb5349956f93b16b74cfe94214e78b44/CURSOR_SKILL.md
repo: Moeblack/ComfyUI-AnimaTool
kind: skill
stars: 109
last_pushed: 2026-03-26T09:47:20Z
license: agpl-3.0
score: 9
domains: [ai-image-generation, mcp-servers, creative-workflows]
tags: [comfyui, anime, prompt-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# Moeblack/ComfyUI-AnimaTool — skill

**Why it's worth keeping:** It utilizes 'negative constraints' to prevent style conflicts and enforces rigid formatting rules (like the '@' prefix) that are essential for specific API success. The structured parameter order and manual/automated verification logic (list-before-use) represent elite agent instruction techniques.

**Summary:** This skill file provides strict operational logic for an agent-driven anime image generation workflow using ComfyUI and the Anima model. It defines high-precision syntax requirements for artists, LoRAs, and prompt hierarchies.

**Source credibility:** High; 109 stars on GitHub suggests a well-regarded community toolset.

**Recency:** Current; updated within the last few months.

**Source:** [Moeblack/ComfyUI-AnimaTool/CURSOR_SKILL.md](https://github.com/Moeblack/ComfyUI-AnimaTool/blob/2a9c5fcbbb5349956f93b16b74cfe94214e78b44/CURSOR_SKILL.md) · 109★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Anima 二次元图像生成

使用 Anima 模型（circlestone-labs/Anima）在本地 ComfyUI 生成高质量二次元/插画图片。

## 触发条件

- 用户要求生成二次元/动漫/插画风格图片
- 用户提到 Anima 模型
- 用户要求使用特定画师风格（如 @fkey, @jima, @wlop）

## 使用方法

**直接调用 MCP 工具** `generate_anima_image`，传入结构化参数。

## 硬性规则

1. **画师必须带 `@` 前缀**（如 `@fkey, @jima`），否则几乎无效
2. **必须明确安全标签**：`safe` / `sensitive` / `nsfw` / `explicit`
3. **推荐画师组合**：`@fkey, @jima`（效果稳定）
4. **标签顺序**：质量 → 人数 → 角色 → 作品 → 画师 → 风格 → 外观 → 标签 → 环境
5. **画师名能用时，`style` 留空**：`style` 只在需要锁品类/媒介时才写（如 `splash art` / `watercolor`）
6. **不要写互斥风格词**：`tags`/`environment` 里不要塞 `chibi` / `lineart` / `flat shading` 这类会抢画师风格的词

## 画师名格式规则

- 必须以 `@` 开头：`@fkey`，而非 `fkey`
- 名字中间**无下划线**：`@kawakami rokkaku`，而非 `@kawakami_rokkaku`
- 多画师用逗号分隔：`@fkey, @jima`（但稳定性下降，建议最多 1-2 位）
- 如果画师名本身含括号（如 `yd (orange maru)`），需要转义：`@yd \(orange maru\)`，避免被解析器误认为附加信息

## LoRA 使用规则

- `loras` 参数接受数组，每项包含 `name`（文件名）和 `weight`（权重，默认 1.0）
- LoRA 仅作用于 UNET（不影响 CLIP），在 UNETLoader → KSampler 之间链式注入
- **`name` 必须与 `list_anima_models(model_type=loras)` 返回值逐字一致**（ComfyUI 会做枚举校验）
- `list_anima_models(model_type=loras)` 仅返回存在同名 `.json` sidecar 元数据文件的 LoRA
- Windows 下路径通常含反斜杠（如 `_Anima\xxx.safetensors`），本工具会自动规范化分隔符
- 远程 ComfyUI 场景下 list 功能不可用（无法读取远程文件系统
```

</details>
