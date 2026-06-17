---
name: Etyamor__Vite-Starter-Theme
source: https://github.com/Etyamor/Vite-Starter-Theme/blob/290b298a998de12345efbd40e95f68c27982005e/CLAUDE.md
repo: Etyamor/Vite-Starter-Theme
kind: claude-md
stars: 37
last_pushed: 2026-03-30T20:06:08Z
license: gpl-2.0
score: 9
domains: [web-frontend, wordpress, build-tools]
tags: [vite, blade, tailwindcss, wordpress-theme]
curated: 2026-06-15
curated_by: config-scout
---

# Etyamor/Vite-Starter-Theme — claude-md

**Why it's worth keeping:** Excellent documentation of the custom asset loading logic and specific workflows for adding templates or assets which prevents AI from making standard WordPress mistakes.

**Summary:** A highly technical guide for a specialized WordPress-Vite-Blade stack that explains non-standard architectural patterns.

**Source credibility:** Decent; 37 stars suggests a useful starter template with recent maintenance.

**Recency:** Current; mentions Tailwind CSS v4 and modern Vite workflows.

**Source:** [Etyamor/Vite-Starter-Theme/CLAUDE.md](https://github.com/Etyamor/Vite-Starter-Theme/blob/290b298a998de12345efbd40e95f68c27982005e/CLAUDE.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance for AI coding assistants when working with code in this repository.

## Project Overview

This is a WordPress theme that uses Vite for asset bundling, Tailwind CSS v4 for styling, and Blade for templating. The theme is designed for minimal complexity with optimized asset handling.

## Development Commands

- `npm run dev` - Start Vite development server with HMR (clears manifest before starting)
- `npm run build` - Build production assets with Vite
- `npm run lint` - Run PHPCS, PHPStan, and Stylelint together
- `npm run lint:php` - Check PHP against PSR-12 coding standards
- `npm run lint:php:fix` - Auto-fix PHPCS violations
- `npm run lint:types` - Run PHPStan static analysis (level 5)
- `npm run lint:css` - Check CSS with Stylelint
- `npm run lint:css:fix` - Auto-fix Stylelint violations
- `npm run typecheck` - Run TypeScript type checking
- `npm run bundle` - Lint + build + create production zip
- `npm run bundle:quick` - Build + zip (skip linting)
- `npm run bundle:clean` - Remove the bundled/ directory

## Blade Templating

The theme uses [jenssegers/blade](https://github.com/jenssegers/blade) (standalone Laravel Blade) for templating.
```

</details>
