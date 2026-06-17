---
name: posit-dev__skills__skill
source: https://github.com/posit-dev/skills/blob/525e989c774a3ae63a300bef7ca3193b291eec2a/shiny/shiny-bslib-theming/SKILL.md
repo: posit-dev/skills
kind: skill
stars: 398
last_pushed: 2026-06-11T16:32:16Z
license: mit
score: 9
domains: [data-science, web-frontend, r-programming]
tags: [shiny, bslib, theming, bootstrap, sass]
curated: 2026-06-15
curated_by: config-scout
---

# posit-dev/skills — skill

**Why it's worth keeping:** It provides a hierarchical customization workflow (presets -> colors -> typography -> Sass) and explains advanced variable injection via the '.where' parameter.

**Summary:** A high-density technical guide for creating professional, production-ready themes in Shiny applications using bslib and Bootstrap 5.

**Source credibility:** High; authored by Garrick Aden-Buie, a leading expert in R/Shiny development at Posit.

**Recency:** Current; utilizes modern Bootstrap 5 and bslib standards.

**Source:** [posit-dev/skills/shiny/shiny-bslib-theming/SKILL.md](https://github.com/posit-dev/skills/blob/525e989c774a3ae63a300bef7ca3193b291eec2a/shiny/shiny-bslib-theming/SKILL.md) · 398★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: shiny-bslib-theming
description: Advanced theming for Shiny apps using bslib and Bootstrap 5. Use when customizing app appearance with bs_theme(), Bootswatch themes, custom colors, typography, brand.yml integration, Bootstrap Sass variables, custom Sass/CSS rules, dark mode and color modes, dynamic theme switching, real-time theming, theme inspection, or making R plots match the app theme with thematic.
metadata:
  author: Garrick Aden-Buie (@gadenbuie)
  version: "1.0"
license: MIT
---

# Theming Shiny Apps with bslib

Customize Shiny app appearance using bslib's Bootstrap 5 theming system. From quick Bootswatch themes to advanced Sass customization and dynamic color mode switching.

## Quick Start

**"shiny" preset (recommended starting point):**
```r
page_sidebar(
  theme = bs_theme(),  # "shiny" preset by default — polished, not plain Bootstrap
  ...
)
```

**Bootswatch theme (for a different visual style):**
```r
page_sidebar(
  theme = bs_theme(preset = "zephyr"),  # or "cosmo", "minty", "darkly", etc.
  ...
)
```

**Custom colors and fonts:**
```r
page_sidebar(
  theme = bs_theme(
    version = 5,
    bg = "#FFFFFF",
    fg = "#333333",
    primary = "#2c3e50",
```

</details>
