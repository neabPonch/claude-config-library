---
name: saas-js__saas-ui
source: https://github.com/saas-js/saas-ui/blob/acf0596b8b41415c4615698ca6698a9c63e3db71/CLAUDE.md
repo: saas-js/saas-ui
kind: claude-md
stars: 1629
last_pushed: 2026-03-06T12:36:10Z
license: mit
score: 9
domains: [web-frontend, monorepo, component-library]
tags: [react, pnpm, design-system]
curated: 2026-06-16
curated_by: config-scout
---

# saas-js/saas-ui — claude-md

**Why it's worth keeping:** The 'Tips for AI Agents' section provides actionable technical shortcuts, while the explicit component file structure template prevents architectural hallucinations.

**Summary:** A comprehensive guide to a complex React monorepo that provides structural clarity and specific build workflows.

**Source credibility:** High; comes from a popular (1.6k stars), actively maintained React design system.

**Recency:** Very current, referencing modern technologies like React 19 and pnpm v10.

**Source:** [saas-js/saas-ui/CLAUDE.md](https://github.com/saas-js/saas-ui/blob/acf0596b8b41415c4615698ca6698a9c63e3db71/CLAUDE.md) · 1629★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Saas UI

## Project Overview

Saas UI is a React component library and design system for SaaS applications.
It's built on top of Chakra UI v3 and Ark UI, providing unstyled primitives
(`@saas-ui/core`) and styled components (`@saas-ui/react`).

**Repository**: https://github.com/saas-js/saas-ui
**Main branch**: `v3`

## Monorepo Structure

This is a pnpm workspaces monorepo orchestrated with Turborepo.

```
apps/
  website/           # Next.js documentation site
  compositions/      # Composition showcase
  palette/           # Palette documentation
packages/
  saas-ui-core/      # Unstyled primitives (GridList, Navbar, Sidebar, Steps, ErrorBoundary)
  saas-ui-react/     # Styled Chakra UI components (30+ components)
  saas-ui-forms/     # React Hook Form + Zod integration
  saas-ui-hooks/     # React hooks library
  saas-ui-modals/    # Modal manager
  saas-ui-auth-provider/ # Authentication provider primitives
  saas-ui-chakra-preset/ # Chakra UI design system preset (recipes, slot-recipes, colors)
  saas-ui-panda-preset/  # Panda CSS preset (experimental)
  saas-ui-tailwind-preset/ # Tailwind CSS preset
  saas-ui-cli/       # CLI tool for scaffolding
  saas-ui-use-
```

</details>
