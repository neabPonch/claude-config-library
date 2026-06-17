---
name: etowahadams__interprot
source: https://github.com/etowahadams/interprot/blob/fae2d3ae90220781289e27a26cb3b0826cf2b07e/CLAUDE.md
repo: etowahadams/interprot
kind: claude-md
stars: 126
last_pushed: 2026-04-23T00:24:40Z
license: mit
score: 8
domains: [web-frontend, data-visualization]
tags: [react, typescript, vite]
curated: 2026-06-15
curated_by: config-scout
---

# etowahadams/interprot — claude-md

**Why it's worth keeping:** The 'Verifying Changes' section provides specific URL patterns that allow an agent to verify work visually, and the architecture section maps key files to their responsibilities.

**Summary:** Provides a clear development workflow for a React frontend including command patterns and architectural mappings.

**Source credibility:** High-quality niche research project with decent star count and recent activity.

**Recency:** Highly current; uses modern toolchain like Vite, pnpm, and React 18.

**Source:** [etowahadams/interprot/CLAUDE.md](https://github.com/etowahadams/interprot/blob/fae2d3ae90220781289e27a26cb3b0826cf2b07e/CLAUDE.md) · 126★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

InterProt is a React frontend for visualizing sparse autoencoder (SAE) features learned from protein language models. It allows researchers to explore interpretable latent features that capture protein structural and functional properties.

- **Website**: https://interprot.com

## Commands

```bash
cd viz
pnpm install        # Install dependencies
pnpm run dev        # Development server at http://localhost:5173
pnpm run build      # Production build (tsc -b && vite build)
pnpm run lint       # ESLint
```

## Verifying Changes

I already have a server runs at http://localhost:5173. Key pages to test:

- **Landing page**: http://localhost:5173/
- **SAE feature viewer**: http://localhost:5173/sae-viz/SAE4096-L24/feature/0 (change feature number to test different features)
- **Custom sequence search**: http://localhost:5173/sae-viz/SAE4096-L24/ (enter a protein sequence to see SAE activations)

Always run `pnpm run build` before committing to catch TypeScript errors.

## Architecture

- **Tech stack**: React 18, TypeScript, Vite, Tailwind CSS, Radix
```

</details>
