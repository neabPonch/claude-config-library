---
name: mnourbina__kadjahealth
source: https://github.com/mnourbina/kadjahealth/blob/b9efa0f51038c23dd82fbe6594f539a9105c6ceb/CLAUDE.md
repo: mnourbina/kadjahealth
kind: claude-md
stars: 0
last_pushed: 2026-05-03T00:05:09Z
license: unknown
score: 7
domains: [web-frontend, prototyping]
tags: [react, monolith, tailwind-v4, single-file]
curated: 2026-06-14
curated_by: config-scout
---

# mnourbina/kadjahealth — claude-md

**Why it's worth keeping:** Explicitly warns the agent against refactoring the monolithic App.tsx structure and provides clear CSS variable mappings for visual consistency.

**Summary:** Defines a mobile-first React prototype that intentionally utilizes a massive single-file architecture with centralized state management.

**Source credibility:** Low star count, but the documentation is highly specific to this unique prototype's constraints.

**Recency:** Current; includes modern tech like Tailwind v4 and Vite-specific environment injections.

**Source:** [mnourbina/kadjahealth/CLAUDE.md](https://github.com/mnourbina/kadjahealth/blob/b9efa0f51038c23dd82fbe6594f539a9105c6ceb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Ce fichier fournit des indications à Claude Code (claude.ai/code) pour travailler dans ce dépôt.

## Présentation du projet

**Kadja Health** est une application React SPA mobile-first pour la gestion de la santé dans le contexte africain (Tchad). C'est un prototype utilisant des données fictives — il n'y a ni backend, ni base de données, ni système d'authentification.

L'application est déployée via **Google AI Studio** (`metadata.json` y fait référence). La `GEMINI_API_KEY` est injectée au moment de l'exécution par AI Studio ; en local, il faut la définir dans `.env.local`.

## Commandes

```bash
npm install          # Installer les dépendances
npm run dev          # Démarrer le serveur de développement sur http://localhost:3000
npm run build        # Build de production (Vite)
npm run preview      # Prévisualiser le build de production
npm run lint         # Vérification TypeScript uniquement (tsc --noEmit)
npm run clean        # Supprimer le dossier dist/
```

Aucune suite de tests n'est configurée.

## Architecture

### Frontend en fichier unique

Toute l'interface est dans **`src/App.tsx`** (~3 300 lignes). C'est intentionnel pour la phase prototype — chaque écra
```

</details>
