---
name: kaptandatasolutions__kaptandatasolutions.github.io
source: https://github.com/kaptandatasolutions/kaptandatasolutions.github.io/blob/497ba48c02b646b38b2d340117268fb43cb52578/CLAUDE.md
repo: kaptandatasolutions/kaptandatasolutions.github.io
kind: claude-md
stars: 0
last_pushed: 2026-06-13T07:34:24Z
license: mit
score: 8
domains: [web-frontend, static-site]
tags: [jekyll, documentation-heavy, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# kaptandatasolutions/kaptandatasolutions.github.io — claude-md

**Why it's worth keeping:** It provides high-level 'recipes' (e.g., how to add a post or translate a page) which enables an agent to understand task intent rather than just file manipulation. It also clearly distinguishes between OS-specific development commands.

**Summary:** A comprehensive operational manual for a Jekyll static site that covers architectural patterns, command structures, and content creation workflows.

**Source credibility:** A specialized professional project with highly specific, non-generic documentation.

**Recency:** Current; references modern Ruby versions and GitHub Actions workflows.

**Source:** [kaptandatasolutions/kaptandatasolutions.github.io/CLAUDE.md](https://github.com/kaptandatasolutions/kaptandatasolutions.github.io/blob/497ba48c02b646b38b2d340117268fb43cb52578/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Ce dépôt est un site web Jekyll statique pour **Kaptan Data Solutions (KDS)**, une entreprise spécialisée dans les solutions data pour la physique médicale. Le site utilise le thème Beautiful Jekyll et sert de blog/portfolio publiant des articles techniques sur la radiothérapie, l'IA, l'automatisation et la data science.

**URL de production**: https://kaptandatasolutions.github.io
**Portfolio démo**: https://kaptan-data-solutions.app/

## Commands de développement

### Développement local

**Windows**:
```bash
serve-site.bat
```

**Unix/Linux/Mac**:
```bash
make serve
```

Ces commandes :
1. Installent automatiquement les dépendances Ruby (`bundle install`)
2. Lancent Jekyll avec livereload sur http://localhost:4000
3. Rechargent automatiquement le navigateur lors des modifications

### Autres commandes utiles

```bash
# Installation/mise à jour des dépendances uniquement
bundle install

# Build du site (génère _site/)
bundle exec jekyll build

# Clean des fichiers générés
make clean  # Unix
# ou supprimer manuellement _site/ et .jekyll-cache/
`
```

</details>
