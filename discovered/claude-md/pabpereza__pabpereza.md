---
name: pabpereza__pabpereza
source: https://github.com/pabpereza/pabpereza/blob/ffd5fb07973a8722d07ed98d381cdea81c558a59/CLAUDE.md
repo: pabpereza/pabpereza
kind: claude-md
stars: 429
last_pushed: 2026-06-14T01:25:33Z
license: apache-2.0
score: 9
domains: [content-ops, web-development]
tags: [docusaurus, workflows, documentation]
curated: 2026-06-14
curated_by: config-scout
---

# pabpereza/pabpereza — claude-md

**Why it's worth keeping:** Uses highly specific skill-to-directory mappings and strict procedural workflows (like the draft-to-publication folder movement) that ensure agentic consistency.

**Summary:** Comprehensive instructions for managing a multi-format educational ecosystem including blogs, technical courses, and YouTube content.

**Source credibility:** High; well-starred and actively maintained personal professional repository.

**Recency:** Current; references modern tech like Docusaurus v3.

**Source:** [pabpereza/pabpereza/CLAUDE.md](https://github.com/pabpereza/pabpereza/blob/ffd5fb07973a8722d07ed98d381cdea81c558a59/CLAUDE.md) · 429★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# GitHub Copilot Instructions

Esta guía proporciona directrices para que los agentes de IA que trabajen en este repositorio de contenido educativo de DevSecOps.

## Arquitectura del Proyecto

Este es un sitio **Docusaurus v3** con:
- **Build automatizado**: `npm run prebuild` genera el grafo de contenido antes de cada build
- **Búsqueda**: Utiliza `docusaurus-lunr-search` para indexación
- **Mermaid**: Soporte para diagramas mediante `@docusaurus/theme-mermaid`
- **Grafo de contenido**: React Force Graph 2D para visualización de relaciones

## Estructura de Contenido

### Blog Posts (`/blog/`)
- IMPORTANTE: Añadr nuevos artículos de blog a la carpeta `blog/.ideas` como borradores iniciales`
- Usar archivo `.md` con nombre del artículo (NO `index.md`)
- Incluir metadatos con `slug`, `authors: pabpereza`, `tags`, `keywords`
- Imágenes en la misma carpeta que el artículo
- Añadir `draft: true` por defecto hasta revisión final
- Evita usar `:` dentro del metadatado de markdown ( title, description, slug, tags... etc)
- **Ejemplo de frontmatter**:
```yaml
---
slug: ruta_devsecops_recomendaciones_2025
title: Ruta DevSecOps, recomendaciones para empezar en 2025
tags: [devsecops, segurida
```

</details>
