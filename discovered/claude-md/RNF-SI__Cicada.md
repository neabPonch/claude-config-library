---
name: RNF-SI__Cicada
source: https://github.com/RNF-SI/Cicada/blob/9ff895ffd6eb31728c22d2a881872cb13b2509c9/claude.md
repo: RNF-SI/Cicada
kind: claude-md
stars: 4
last_pushed: 2026-06-15T15:14:29Z
license: gpl-3.0
score: 8
domains: [web-app, fullstack, backend-api]
tags: [django, angular, postgis, rbac]
curated: 2026-06-15
curated_by: config-scout
---

# RNF-SI/Cicada — claude-md

**Why it's worth keeping:** It provides explicit file structure maps for navigation and actual database model snippets to ground the LLM in schema relationships before it starts coding.

**Summary:** A highly detailed project manual covering the full stack, directory hierarchy, and complex business logic regarding user roles.

**Source credibility:** Active repository (updated 0 months ago) with high technical detail.

**Recency:** Highly modern, citing cutting-edge versions like Angular 19 and Django 5.0.

**Source:** [RNF-SI/Cicada/claude.md](https://github.com/RNF-SI/Cicada/blob/9ff895ffd6eb31728c22d2a881872cb13b2509c9/claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 🌿 Application de Gestion des Plans de Gestion

## 📋 Contexte du projet

Application web développée pour le CEN (Conservatoire d'Espaces Naturels) et RNF (Réserves Naturelles de France) permettant la gestion des plans de gestion d'espaces naturels avec support géospatial.


### Repository
- **GitHub** : https://github.com/RNF-SI/Cicada
- **Branches** : main (production), develop (développement), feature/* (fonctionnalités)

## 🛠️ Stack technique

### Backend
- **Python 3.11+**
- **Django 5.0+** - Framework web principal
- **Django REST Framework 3.14+** - API REST
- **PostgreSQL 15+** - Base de données principale
- **PostGIS 3.3+** - Extension géospatiale
- **Redis 7+** - Cache et broker de messages
- **Celery** (optionnel V1) - Tâches asynchrones

### Frontend  
- **Angular 19+** - Framework SPA
- **TypeScript 5+** - Langage principal
- **Angular Material** - Composants UI
- **RxJS** - Programmation réactive
- **Leaflet** - Cartes interactives
- **SCSS** - Styles

### Infrastructure
- **Docker & Docker Compose** - Conteneurisation
- **GitHub Actions** - CI/CD
- **Apache** - Reverse proxy (production)
- **Gunicorn** - WSGI server (production)

### Outils de développement
- **Black
```

</details>
