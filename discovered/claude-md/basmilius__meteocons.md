---
name: basmilius__meteocons
source: https://github.com/basmilius/meteocons/blob/70dfb1d6e30dc9e791cfb0e4c5b5e5e60e972aa0/CLAUDE.md
repo: basmilius/meteocons
kind: claude-md
stars: 1568
last_pushed: 2026-04-12T19:52:41Z
license: mit
score: 9
domains: [design-engineering, asset-pipelines, web-graphics]
tags: [svg, lottie, figma, animation, monorepo]
curated: 2026-06-14
curated_by: config-scout
---

# basmilius/meteocons — claude-md

**Why it's worth keeping:** Provides exact command mappings, deep technical data-flow diagrams (Figma to output), and precise JSON schema definitions for animation logic.

**Summary:** A highly detailed architectural blueprint for a complex asset pipeline that transforms Figma designs into animated SVG and Lottie packages.

**Source credibility:** Highly credible; high star count (1.5k) and recently maintained.

**Recency:** 

**Source:** [basmilius/meteocons/CLAUDE.md](https://github.com/basmilius/meteocons/blob/70dfb1d6e30dc9e791cfb0e4c5b5e5e60e972aa0/CLAUDE.md) · 1568★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Meteocons

Monorepo voor Meteocons: animated weather icons. Bevat de export pipeline, publishable icon packages en documentatie.

## Monorepo structuur

```
packages/
├── exporter/     # @meteocons/exporter  — Figma → SVG/Lottie export pipeline
├── svg/          # @meteocons/svg       — Publishable animated SVG icon package
├── svg-static/   # @meteocons/svg-static — Publishable static SVG icon package (no SMIL animations)
├── lottie/       # @meteocons/lottie    — Publishable Lottie icon package
└── docs/         # @meteocons/docs      — Astro docs + marketing website
```

## Commando's

```bash
bun run fetch              # Haal SVGs op uit Figma (gebruikt cache)
bun run fetch --force      # Forceer opnieuw downloaden
bun run export             # Exporteer alle iconen (SVG + Lottie)
bun run export --frame X   # Exporteer één icoon
bun run validate           # Valideer layer-namen en coverage
bun run publish-icons      # Kopieer output naar @meteocons/svg, @meteocons/svg-static en @meteocons/lottie
bun run docs:dev           # Start docs website dev server
```

## Architectuur

```
Figma → fetch → packages/exporter/.cache/svgs/   (statische SVGs)
                    ↓
animations/
```

</details>
