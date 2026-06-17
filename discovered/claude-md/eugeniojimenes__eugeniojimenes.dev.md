---
name: eugeniojimenes__eugeniojimenes.dev
source: https://github.com/eugeniojimenes/eugeniojimenes.dev/blob/5cda718f5d8d67cada15edd98289fa10a247e3ff/CLAUDE.md
repo: eugeniojimenes/eugeniojimenes.dev
kind: claude-md
stars: 1
last_pushed: 2026-05-25T17:52:22Z
license: bsd-3-clause
score: 9
domains: [web-frontend, static-site-generator]
tags: [jekyll, tailwind-v4, hotwire, i18n]
curated: 2026-06-15
curated_by: config-scout
---

# eugeniojimenes/eugeniojimenes.dev — claude-md

**Why it's worth keeping:** It provides exact front-matter requirements for bilingual posts and explicitly defines the asset pipeline to prevent breaking the Webpack/Jekyll build sequence.

**Summary:** A highly detailed guide for a specialized Jekyll, Tailwind v4, and Hotwire stack that emphasizes strict content and build patterns.

**Source credibility:** A personal technical blog using modern, up-to-date web technologies.

**Recency:** Extremely recent; updated within the last month and uses Tailwind v4.

**Source:** [eugeniojimenes/eugeniojimenes.dev/CLAUDE.md](https://github.com/eugeniojimenes/eugeniojimenes.dev/blob/5cda718f5d8d67cada15edd98289fa10a247e3ff/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Personal blog at https://eugeniojimenes.dev — Jekyll + Tailwind v4 + Hotwire, deployed on Netlify. Terminal-flavored UI, Tokyo Night dark theme by default with a beige light mode. This file orients Claude (and future-me) on conventions and workflows specific to this repo.

## Stack snapshot

- **Static generator:** Jekyll 4.3.x (`src/` source → `src/_site/` output)
- **Styling:** Tailwind CSS 4.x (CSS-first `@theme` config in `src/assets/main.css`, `@tailwindcss/webpack` loader, dark mode via `class` strategy through `@custom-variant`)
- **JS:** Hotwire (Turbo 8.x, Stimulus 3.2.x) bundled by Webpack 5 — page morphing + View Transitions enabled via `<meta>` tags in `_layouts/default.html`
- **Plugins:** `jekyll-paginate-v2`, `jekyll-seo-tag`, `jekyll-sitemap`
- **Ruby:** 3.4.9 (`.ruby-version`, `mise.toml`) — managed via Bundler
- **Node:** 22 LTS / NPM 10 (per `netlify.toml`, `mise.toml`)
- **Hosting:** Netlify (`netlify.toml` drives build)
- **Process manager:** Foreman via `Procfile.dev`

See "Upgrade backlog" at bottom — most pins are behind latest.

## Repo layout

```
src/
├── _config.yml           # Jekyll site config (EN is default locale)
├── _data/
│   ├── tra
```

</details>
