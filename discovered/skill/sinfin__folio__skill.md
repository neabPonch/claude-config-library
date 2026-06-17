---
name: sinfin__folio__skill
source: https://github.com/sinfin/folio/blob/e3ca3418780b62d670a11c4218259176491d4189/.skills/folio-scss/SKILL.md
repo: sinfin/folio
kind: skill
stars: 10
last_pushed: 2026-06-15T14:03:14Z
license: mit
score: 8
domains: [web-frontend, css]
tags: [sass, bem, component-driven-development, styling-conventions]
curated: 2026-06-15
curated_by: config-scout
---

# sinfin/folio — skill

**Why it's worth keeping:** Provides excellent 'Good vs Bad' examples for component isolation and promotes modern container queries over media queries.

**Summary:** Defines strict BEM-based Sass/SCSS styling conventions for a component-driven architecture.

**Source credibility:** Low star count suggests this is a highly specialized design system specification rather than a generic tutorial.

**Recency:** Highly current, specifically through its emphasis on responsive container queries.

**Source:** [sinfin/folio/.skills/folio-scss/SKILL.md](https://github.com/sinfin/folio/blob/e3ca3418780b62d670a11c4218259176491d4189/.skills/folio-scss/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: folio-scss
description: >-
  Sass/SCSS styling conventions for Folio components: BEM nesting with &,
  colocated component stylesheets, scoping rules, and avoiding cross-component
  styling. Use when writing or editing .sass/.scss files, styling ViewComponents,
  or when the user asks about CSS/Sass conventions in Folio.
---

# Sass styling (Folio)

## Styles belong on components

Almost all styles should live in **colocated component stylesheets** (`_component.sass` next to the Ruby/Slim file). Standalone stylesheets outside `app/components` should be rare — reserved for global resets, variables, or third-party overrides.

## BEM nesting

Use the block class as the root selector, then **`&__element`** and **`&--modifier`** nesting:

```sass
.f-c-ui-button
  display: inline-flex
  align-items: center

  &__icon
    margin-left: -4px

  &__label
    font-weight: $font-weight-bold

  &--primary
    background: $blue
    color: $white

  &--primary &__label
    text-transform: uppercase
```

- **One root selector** per component file — the BEM block.
- **Elements** (`&__`) and **modifiers** (`&--`) are always nested under the block.
- For modifier + element combinations, use
```

</details>
