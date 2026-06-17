---
name: Hawk-on__Blog__blog-skill
source: https://github.com/Hawk-on/Blog/blob/96030d55641f460b25d90296b4886169e48eb9d4/.claude/blog-skill.md
repo: Hawk-on/Blog
kind: skill
stars: 0
last_pushed: 2026-05-09T23:47:30Z
license: unknown
score: 8
domains: [web-frontend, content-management]
tags: [astro, style-guide, documentation]
curated: 2026-06-16
curated_by: config-scout
---

# Hawk-on/Blog — skill

**Why it's worth keeping:** It provides highly specific instructions like slug normalization rules (special character mapping) and a detailed CSS design system that prevents styling hallucinations. It also bridges the gap between code and content by defining citation and tone standards.

**Summary:** A comprehensive technical and stylistic manual for an Astro-based blog, covering file architecture, data schemas, and UI patterns.

**Source credibility:** Low-profile personal project (0 stars).

**Recency:** Current, referencing Astro 6.x.

**Source:** [Hawk-on/Blog/.claude/blog-skill.md](https://github.com/Hawk-on/Blog/blob/96030d55641f460b25d90296b4886169e48eb9d4/.claude/blog-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Blogg-referanse for Claude

Rask oppslagsguide for denne bloggens tekniske struktur, stilmønster og konvensjonar.
Bruk denne fila for å sleppe å re-utforska kodebasen i nye sesjonar.

---

## Teknisk stack

- **Framework:** Astro 6.x (Content Layer), statisk HTML/CSS
- **Hosting:** GitHub Pages via GitHub Actions
- **Innhald:** Markdown-filer (`.md`) i `src/content/blog/`
- **Ingen JS-framework** — berre Astro og `@astrojs/rss` (med React Islands for spesifikke komponentar)

---

## Filstruktur

```
src/
├── content/
│   └── blog/
│       └── *.md             # Blogginnlegg
├── content.config.ts        # Schema for innhaldssamlingar
├── layouts/
│   ├── Grunnoppsett.astro   # Hovudlayout (header, footer, tema-bryter)
│   └── Artikkel.astro       # Artikkellayout (innhaldstabell, leseprosessbar)
├── pages/
│   ├── index.astro          # Startsida (listar alle .md-innlegg)
│   ├── om.astro             # Om-sida
│   ├── 404.astro            # 404-side
│   ├── rss.xml.ts           # RSS-feed
│   ├── tag/[tag].astro      # Dynamiske tag-sider
│   └── [slug].astro         # Dynamisk ruting for blogginnlegg
├── styles/
│   └── global.css           # All CSS (éi fil, ingen komponent-CSS)
```

</details>
