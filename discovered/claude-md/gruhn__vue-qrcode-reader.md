---
name: gruhn__vue-qrcode-reader
source: https://github.com/gruhn/vue-qrcode-reader/blob/ce28111a7390c3ccb0482bcd9f949adfeafdff72/CLAUDE.md
repo: gruhn/vue-qrcode-reader
kind: claude-md
stars: 2306
last_pushed: 2025-07-23T11:14:35Z
license: mit
score: 7
domains: [web-frontend, vuejs]
tags: [architecture, build-system, typescript]
curated: 2026-06-17
curated_by: config-scout
---

# gruhn/vue-qrcode-reader — claude-md

**Why it's worth keeping:** Effective at categorizing module responsibilities (Core vs Utility) and providing critical build constraints like external dependency management.

**Summary:** Provides a high-density architectural map and essential build/documentation commands for a Vue 3 component library.

**Source credibility:** High; part of a popular, well-starred open-source project (2.3k+ stars).

**Recency:** Current; utilizes modern toolchains like pnpm v8 and Vite.

**Source:** [gruhn/vue-qrcode-reader/CLAUDE.md](https://github.com/gruhn/vue-qrcode-reader/blob/ce28111a7390c3ccb0482bcd9f949adfeafdff72/CLAUDE.md) · 2306★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

**Build**: `pnpm run build` - Compiles the library using Vite
**Type Check**: `pnpm run type-check` - Runs Vue TypeScript compiler without emitting files
**Format**: `pnpm run format` - Formats code using Prettier (Vue, TS, JSON, MD files)
**Documentation**: 
- `pnpm run docs:dev` - Starts VitePress dev server for documentation
- `pnpm run docs:build` - Builds documentation
- `pnpm run docs:preview` - Previews built documentation

**Package Manager**: Uses pnpm (v8.3.1) - always use `pnpm` instead of `npm`

## Architecture Overview

This is a Vue 3 QR code/barcode scanning library with three main components:

### Core Components (`src/components/`)
- **QrcodeStream.vue**: Continuous camera stream scanning using WebRTC
- **QrcodeCapture.vue**: File upload scanning (click to select files)
- **QrcodeDropZone.vue**: Drag-and-drop file scanning

### Utility Modules (`src/misc/`)
- **scanner.ts**: Core barcode detection logic using `barcode-detector` library
- **camera.ts**: Camera management, device selection, and constraints
- **errors.ts**: Cent
```

</details>
