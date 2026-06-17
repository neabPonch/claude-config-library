---
name: luisguzmanverbena__projects__claude
source: https://github.com/luisguzmanverbena/projects/blob/7d9223836872350041876f35e116738a849ae1c0/Helios%20Design%20System%20Reference/claude.md
repo: luisguzmanverbena/projects
kind: claude-md
stars: 0
last_pushed: 2026-03-15T23:20:18Z
license: unknown
score: 8
domains: [web-frontend, design-system]
tags: [ember, react, css-tokens, ui-components]
curated: 2026-06-15
curated_by: config-scout
---

# luisguzmanverbena/projects — claude-md

**Why it's worth keeping:** It provides exact syntax signatures (e.g., <Hds::Button @text='...' />) and configuration steps that prevent AI hallucinations when generating UI code.

**Summary:** A highly structured technical reference for the Helios design system, detailing component usage, installation, and CSS token patterns.

**Source credibility:** High-quality documentation consistent with professional enterprise design system standards.

**Recency:** Current, utilizing modern package managers (pnpm) and component patterns.

**Source:** [luisguzmanverbena/projects/Helios Design System Reference/claude.md](https://github.com/luisguzmanverbena/projects/blob/7d9223836872350041876f35e116738a849ae1c0/Helios%20Design%20System%20Reference/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Helios Design System Reference

Helios is HashiCorp's design system, providing design tokens, icons, and components maintained in a monorepo and published to npm.

Official documentation: https://helios.hashicorp.design

---

## Quick Reference

### Packages

- **@hashicorp/design-system-components** - Ember components with Sass/CSS styles
- **@hashicorp/design-system-tokens** - Design tokens (colors, typography, elevation, spacing)
- **@hashicorp/flight-icons** - Icon library (can be used independently)

### Installation

```bash
# Components (includes tokens and CSS helpers)
pnpm add @hashicorp/design-system-components

# Tokens only
pnpm add @hashicorp/design-system-tokens

# Icons only (for React or standalone use)
pnpm add @hashicorp/flight-icons
```

---

## Ember Setup

### 1. Install Components

```bash
pnpm add @hashicorp/design-system-components
```

### 2. Choose Style Import Method

**Option A: Sass (recommended)**

Install Sass preprocessor:
```bash
ember install ember-cli-sass
```

Rename `app/styles/app.css` to `app/styles/app.scss`

Add to `ember-cli-build.js`:
```js
sassOptions: {
  precision: 4,
  includePaths: [
    './node_modules/@hashicorp/design-system-toke
```

</details>
