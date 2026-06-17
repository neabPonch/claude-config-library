---
name: 21saul__PROYECTO_FINAL_NMONZZON
source: https://github.com/21saul/PROYECTO_FINAL_NMONZZON/blob/eeee2436d9aed81b10ec5d0bc0916ff252265d88/claude.md
repo: 21saul/PROYECTO_FINAL_NMONZZON
kind: claude-md
stars: 0
last_pushed: 2026-04-28T13:03:06Z
license: mit
score: 8
domains: [web-frontend, full-stack-php, devops]
tags: [ddev, codeigniter, css-architecture, senior-guidelines]
curated: 2026-06-16
curated_by: config-scout
---

# 21saul/PROYECTO_FINAL_NMONZZON — claude-md

**Why it's worth keeping:** Includes environment-specific execution patterns (DDEV/WSL2) and explicit 'Senior' architectural rules to prevent CSS specificity issues. It treats the LLM as a specialist rather than just a code generator.

**Summary:** Establishes a specific technical stack, file architecture, and high-standard frontend guidelines for a full-stack PHP project.

**Source credibility:** Single developer repository with low social proof, but high technical density.

**Recency:** Extremely current, referencing PHP 8.4 and modern development workflows.

**Source:** [21saul/PROYECTO_FINAL_NMONZZON/claude.md](https://github.com/21saul/PROYECTO_FINAL_NMONZZON/blob/eeee2436d9aed81b10ec5d0bc0916ff252265d88/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - NMONZZON STUDIO Context & Senior Frontend Guidelines

Este archivo proporciona el contexto técnico y las reglas de comportamiento para el desarrollo de la plataforma web de la artista **NMONZZON**.

## 1. Visión General del Proyecto
**NMONZZON STUDIO** es una aplicación Full-Stack que combina un portafolio artístico, e-commerce (Stripe), configurador de retratos a medida y gestión de eventos.

- **Stack Principal:** CodeIgniter 4.7.x, PHP 8.4, MariaDB 11.8.
- **Entorno:** DDEV sobre WSL2 (Ubuntu).
- **Frontend Core:** Bootstrap 5.3.3, GSAP (animaciones), AOS (scroll), Masonry (galerías).
- **Infraestructura:** API REST con JWT, Integración n8n, PWA, y Cloudinary para imágenes.

## 2. Estructura de Archivos Clave
- `app/Controllers/`: Divididos en `Api/`, `Web/` y `Admin/`.
- `app/Views/`: Layouts principales en `layouts/main.php` (público) y `admin.php` (panel).
- `public/assets/`: 
  - `css/custom.css`: Estilos personalizados (+2000 líneas).
  - `js/portrait-config.js`: Lógica del configurador de retratos.
  - `js/app.js`: Registro de Service Worker y lógica global.

## 3. Directrices para el "Senior Frontend Developer" (Tu Rol Especializado)
Para resolver los proble
```

</details>
