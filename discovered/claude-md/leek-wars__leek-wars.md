---
name: leek-wars__leek-wars
source: https://github.com/leek-wars/leek-wars/blob/989a77c88ad965bda3fe829c886ce5a2adf07698/CLAUDE.md
repo: leek-wars/leek-wars
kind: claude-md
stars: 191
last_pushed: 2026-06-14T17:09:23Z
license: gpl-3.0
score: 8
domains: [web-frontend, ui-ux]
tags: [vuejs, typescript, i18n, design-system]
curated: 2026-06-15
curated_by: config-scout
---

# leek-wars/leek-wars — claude-md

**Why it's worth keeping:** The file provides excellent patterns for preventing AI hallucinations via a project-specific 'Terminology' section and strictly enforces the use of design system variables over hardcoded colors.

**Summary:** Establishes strict protocols for changelog updates, domain-specific terminology mapping, and CSS variable usage to maintain UI consistency.

**Source credibility:** Reliable source; active repository with high recent maintenance.

**Recency:** Extremely current, referencing modern tools like Vite 7.

**Source:** [leek-wars/leek-wars/CLAUDE.md](https://github.com/leek-wars/leek-wars/blob/989a77c88ad965bda3fe829c886ce5a2adf07698/CLAUDE.md) · 191★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Instructions pour Claude Code - Leek Wars Client

## Structure du projet

- **Frontend Vue.js 3** (Composition API, `<script setup>`) avec TypeScript, **Vite 7** et **Vuetify 3**
- **Éditeur de code** : Monaco Editor (`src/component/editor/`)
- **Points d'entrée** : `index.html` charge `src/lang/locale/<lang>.ts` (traductions) puis `src/main.ts` (app). `main.ts` importe `src/model/vue.ts` qui bootstrappe l'app via `createApp`.

## Changelogs

Les changelogs sont dans `src/component/changelog/` au format YAML.

### Fichiers principaux
- `changelog.fr.yaml` - Version française (principale)
- `changelog.en.yaml` - Version anglaise

### Format
```yaml
<version>:
  title: "Titre de la version"
  added:
    - "Nouvelle fonctionnalité. #img_<version>_<nom>"
  improved:
    - "Amélioration existante."
  fixed:
    - "Correction de bug."
```

### Règles
- Toujours mettre à jour **FR, EN et IT** ensemble
- Les images sont référencées avec `#img_<version>_<nom>`
- La version en cours de développement a le titre "WIP"
- Créditer les contributeurs avec "(merci à <pseudo>)"

## Terminologie du jeu
- **Potager** (pas "Jardin") : page de matchmaking et lancement de combat.
- **Habs** (pas "HABs"
```

</details>
