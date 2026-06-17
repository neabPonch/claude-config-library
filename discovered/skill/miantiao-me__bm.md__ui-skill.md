---
name: miantiao-me__bm.md__ui-skill
source: https://github.com/miantiao-me/bm.md/blob/a3dade1a390f45975418706bbbb2d8c4af8efca3/docs/ui-skill.md
repo: miantiao-me/bm.md
kind: skill
stars: 589
last_pushed: 2026-04-29T12:56:19Z
license: agpl-3.0
score: 9
domains: [web-frontend, react, tailwind-css]
tags: [ui-design-system, animation-best-practices, frontend-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# miantiao-me/bm.md — skill

**Why it's worth keeping:** It utilizes specific 'negative constraints' (e.g., forbidding layout animations or large blurs) and modern unit preferences like `h-dvh` which significantly reduces agent-generated UI jank.

**Summary:** A highly opinionated set of technical constraints for building high-performance React/Tailwind CSS interfaces.

**Source credibility:** High; the repository is well-starred and shows recent activity.

**Recency:** Very current, including up-to-date library names like `motion/react`.

**Source:** [miantiao-me/bm.md/docs/ui-skill.md](https://github.com/miantiao-me/bm.md/blob/a3dade1a390f45975418706bbbb2d8c4af8efca3/docs/ui-skill.md) · 589★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# UI Skills

用于与智能代理构建更好界面的有明确设计取向的约束。

## Stack

- MUST 在使用自定义值之前使用 Tailwind CSS 或者 shadcn-ui 的默认值（间距、圆角、阴影）
- MUST 在需要 JavaScript 动画时使用 `motion/react`（原名 `framer-motion`）
- SHOULD 在 Tailwind CSS 中为入场和微动画使用 `tw-animate-css`
- 必须使用 `cn` 工具（`clsx` + `tailwind-merge`）来处理类名逻辑

## Components

- 必须为任何涉及键盘或焦点行为的场景使用可访问的组件原语（`Base UI`、`React Aria`）
- 必须首先使用项目现有的组件原语
- 绝不在同一交互面内混用原语系统
- 如果与技术栈兼容，应优先选择 [`Base UI`](https://base-ui.com/react/components) 作为新的原语
- 必须为仅图标按钮添加一个 `aria-label`
- 除非有明确要求，否则绝对不要手动重建键盘或焦点行为

## Interaction

- 必须为破坏性或不可逆的操作使用 `AlertDialog`
- 应该在加载状态下使用结构化骨架屏
- 切勿使用 `h-screen`，改用 `h-dvh`
- 固定元素必须尊重 `safe-area-inset`
- 必须在发生操作的位置旁显示错误信息
- 切勿在 `input` 或 `textarea` 元素中阻止粘贴

## Animation

- 除非有明确要求，否则切勿添加动画
- 必须仅对合成器属性（`transform`、`opacity`）进行动画
- 切勿对布局属性（`width`、`height`、`top`、`left`、`margin`、`padding`）进行动画
- 应避免对绘制属性（`background`、`color`）进行动画，除非用于小型局部 UI（文本、图标）
- 进入时应使用 `ease-out`
- 交互反馈的时长绝不可超过 `200ms`
- 当不在屏幕上时必须暂停循环动画
- 必须遵守 `prefers-reduced-motion`
- 除非有明确要求，否则绝不引入自定义缓动曲线
- 应避免对大型图像或全屏画面进行动画处理

## Typography

- 必须为数据使用 `tabular-nums`
- 应该在密集型 UI 中使用 `truncate` 或 `line-clamp`
- 切勿修改 `letter-spacing`（`tracking-`），除非有明确请求

## Layout

- 必须使用固定的 `z-index` 刻度（不得使用任意的 `z-x`）
```

</details>
