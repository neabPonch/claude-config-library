---
name: hadyfayed__filament-react-wrapper
source: https://github.com/hadyfayed/filament-react-wrapper/blob/63acceea51f41389b8b3994c81fb22e41927a99e/CLAUDE.md
repo: hadyfayed/filament-react-wrapper
kind: claude-md
stars: 1
last_pushed: 2025-07-15T23:20:39Z
license: mit
score: 9
domains: [web-frontend, backend-api, fullstack-frameworks]
tags: [dual-package, laravel, react, architecture-patterns]
curated: 2026-06-17
curated_by: config-scout
---

# hadyfayed/filament-react-wrapper — claude-md

**Why it's worth keeping:** The 'Architecture Patterns' section provides concrete code snippets for extending the system; it also bridges the gap between different ecosystems (NPM and Composer) with clear command mappings.

**Summary:** Provides high-density structural context for a complex dual-stack (PHP/JS) architecture.

**Source credibility:** Single-star repo, but demonstrates professional-grade architectural documentation typical of high-end packages.

**Recency:** Highly current, utilizing modern tooling like Vite, Vitest, and ESLint flat config.

**Source:** [hadyfayed/filament-react-wrapper/CLAUDE.md](https://github.com/hadyfayed/filament-react-wrapper/blob/63acceea51f41389b8b3994c81fb22e41927a99e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a React Wrapper package for Laravel/Filament applications - an enterprise-grade React integration system that provides seamless component registration, state management, and real-time synchronization. It's both an NPM package (@hadyfayed/filament-react-wrapper) and a Composer package (hadyfayed/filament-react-wrapper).

## Architecture

### Dual Package Structure
- **NPM Package**: TypeScript/React components and services in `resources/js/`
- **Composer Package**: PHP Laravel/Filament integration in `src/`
- **Hybrid Build**: Produces both ES modules for NPM and Laravel-specific bundles

### Core Components

#### React/TypeScript Side (`resources/js/`)
- **Main Entry**: `index.tsx` - Central export point for all functionality
- **Component Registry**: `components/ReactComponentRegistry.tsx` - Dynamic component registration system
- **Universal Renderer**: `components/UniversalReactRenderer.tsx` - Renders components from DOM attributes
- **State Manager**: `components/StateManager.tsx` - Global state management with React context
- **Filam
```

</details>
