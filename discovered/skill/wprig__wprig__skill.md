---
name: wprig__wprig__skill
source: https://github.com/wprig/wprig/blob/4d5c6fc01bef7ea0bad8b955c7fe64d409b52d72/.ai/skills/styles/SKILL.md
repo: wprig/wprig
kind: skill
stars: 1321
last_pushed: 2026-05-26T23:42:13Z
license: gpl-3.0
score: 8
domains: [web-frontend, wordpress, testing]
tags: [css, playwright, visual-regression, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# wprig/wprig — skill

**Why it's worth keeping:** It defines a specific 'Ralph Loop' ritual using Playwright commands that an agent can execute to verify visual changes, preventing regressions.

**Summary:** A specialized guide for managing CSS workflows, build processes, and visual regression testing within the WP Rig WordPress theme.

**Source credibility:** High; the source is a popular-starred, professional-grade WordPress development toolkit.

**Recency:** Current; uses modern CSS patterns and integrates contemporary end-to-end testing workflows.

**Source:** [wprig/wprig/.ai/skills/styles/SKILL.md](https://github.com/wprig/wprig/blob/4d5c6fc01bef7ea0bad8b955c7fe64d409b52d72/.ai/skills/styles/SKILL.md) · 1321★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Guide to managing CSS styles, partials, and builds in WP Rig.
globs: assets/css/src/**/*.css, build-css.js
---

# WP Rig Styles & CSS

This guide describes how to work with CSS in WP Rig.

## Configuration & Features

Before writing or modifying CSS, you **MUST** reference the `config/config.json`.

*   **CSS Preloading:** Check `dev.styles.preload` for files automatically injected into every compiled CSS file (e.g., `_custom-media.css`). Avoid redundant `@import` statements for these files.

## CSS Structure

Source files are in `assets/css/src/` and processed by `build-css.js`.
All CSS files are built into `assets/css/` if they are not prefixed with a `_`.


## Common Style Tasks

### Change the header styles

1. Edit `assets/css/src/_header.css`
2. Run `npm run dev` to rebuild and watch
3. Header styles are imported via `global.css`

### Add a new CSS partial

1. Create `assets/css/src/_yourfile.css`
2. Import it in the relevant css file (ex. `assets/css/src/global.css`) with `@import "_yourfile.css";`
3. Run `npm run dev` to rebuild if dev server is not already running

## Visual Verification (Ralph Loop)

For visual changes, use Playwright to ensure regression
```

</details>
