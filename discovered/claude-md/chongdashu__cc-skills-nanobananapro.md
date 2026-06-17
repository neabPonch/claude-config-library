---
name: chongdashu__cc-skills-nanobananapro
source: https://github.com/chongdashu/cc-skills-nanobananapro/blob/6e8a27f335063633bff66c63fe6b8913480623c0/CLAUDE.md
repo: chongdashu/cc-skills-nanobananapro
kind: claude-md
stars: 138
last_pushed: 2025-12-25T00:44:25Z
license: unknown
score: 8
domains: [web-frontend, ai-integration, threejs]
tags: [nextjs, threejs, gemini, high-context]
curated: 2026-06-17
curated_by: config-scout
---

# chongdashu/cc-skills-nanobananapro — claude-md

**Why it's worth keeping:** It includes crucial implementation details like UV mapping coordinates and dynamic import patterns that prevent an agent from breaking fragile 3D logic; the 'Available Skills' section also defines project-specific expert personas.

**Summary:** A high-context configuration for a specialized Next.js/Three.js application that bridges architectural intent with low-level implementation constraints.

**Source credibility:** Good star count for a niche/demo repository suggests successful community interest.

**Recency:** Current with modern Next.js and AI tool workflows.

**Source:** [chongdashu/cc-skills-nanobananapro/CLAUDE.md](https://github.com/chongdashu/cc-skills-nanobananapro/blob/6e8a27f335063633bff66c63fe6b8913480623c0/CLAUDE.md) · 138★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chinese New Year Card Generator - A Next.js 15 app that transforms photos into festive Lunar New Year cards using Google Gemini image generation, with an interactive 3D card preview.

## Commands

```bash
npm run dev      # Start dev server at localhost:3000
npm run build    # Production build
npm run start    # Run production server
npm run lint     # Run Next.js linter
```

## Architecture

### Data Flow
1. User uploads selfie → FileReader converts to base64
2. Server action calls Gemini API → generates 16:9 two-panel card image
3. Image displayed in UI → user can trigger 3D preview or download

### Key Files
- `app/page.tsx` - Main UI with upload zone, loading states, result display, snowfall effect
- `app/actions/generate.ts` - Server action using `gemini-3-pro-image-preview` model
- `app/components/Card3DPreview.tsx` - Three.js fold-out card with OrbitControls

### AI Model
Always use exact model string: `gemini-3-pro-image-preview` (Nano Banana Pro)

### Three.js Pattern
Uses dynamic imports (`await import('three')`) for code splitting. The
```

</details>
