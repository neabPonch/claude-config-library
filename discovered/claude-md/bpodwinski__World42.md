---
name: bpodwinski__World42
source: https://github.com/bpodwinski/World42/blob/bacbeddf8d4d231120f98c24eaaa3503e51ab775/CLAUDE.md
repo: bpodwinski/World42
kind: claude-md
stars: 6
last_pushed: 2026-03-19T22:13:11Z
license: unknown
score: 9
domains: [web-graphics, game-engine]
tags: [typescript, rust-wasm, math-intensive]
curated: 2026-06-14
curated_by: config-scout
---

# bpodwinski/World42 — claude-md

**Why it's worth keeping:** The 'Golden Rules' section on coordinate spaces is a perfect example of providing critical domain context to prevent math errors, alongside explicit dependency-direction mapping.

**Summary:** A high-density technical manual for a planetary rendering engine that defines strict architectural layers and complex mathematical constraints.

**Source credibility:** Highly professional/specialized content from a niche WebGL/WASM project.

**Recency:** Very recent (3 months ago) and utilizes modern toolchains like Rspack and WebGPU.

**Source:** [bpodwinski/World42/CLAUDE.md](https://github.com/bpodwinski/World42/blob/bacbeddf8d4d231120f98c24eaaa3503e51ab775/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Vue d'ensemble

**World42** est un moteur de rendu planétaire temps réel 1:1, conçu pour explorer des surfaces planétaires à toute altitude (du sol jusqu'à l'espace). Il implémente un système CDLOD (Continuous Distance-based Level of Detail) par quadtree sur une quad-sphère, avec une caméra à origine flottante pour maintenir la précision numérique aux échelles interplanétaires.

- **Version :** 0.0.5
- **Demo live :** https://bpodwinski.github.io/World42/
- **Type :** SPA statique (pas de serveur, pas de base de données)

---

## Tech stack

| Composant | Technologie | Version |
|-----------|-------------|---------|
| Rendu 3D | BabylonJS | 8.51.1 |
| Langage principal | TypeScript (strict) | ESNext |
| Terrain procédural | Rust + wasm-bindgen | edition 2024 |
| Bruit de terrain | `noise` crate (Perlin/Simplex) | 0.9 |
| Bundler | Rspack | 1.5.8 |
| Tests unitaires | Vitest | 4.0.5 |
| Tests E2E | Playwright (scripts custom) | — |
| Rendu GPU | WebGPU (fallback WebGL2) | — |
| Déploiement | GitHub Pages | — |

---

## Commandes de développement

```bash
# TypeScri
```

</details>
