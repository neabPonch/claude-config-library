---
name: K41R0N__Figaro-Design-Library
source: https://github.com/K41R0N/Figaro-Design-Library/blob/b86e43669a5a88a6de48dc51aaf41f64dd27c47a/Claude.md
repo: K41R0N/Figaro-Design-Library
kind: claude-md
stars: 0
last_pushed: 2025-11-17T21:04:24Z
license: unknown
score: 8
domains: [web-frontend, architecture]
tags: [technical-debt, type-safety, architectural-context]
curated: 2026-06-16
curated_by: config-scout
---

# K41R0N/Figaro-Design-Library — claude-md

**Why it's worth keeping:** The 'Current Issues & Root Causes' section is a perfect pattern for CLAUDE.md; it provides an AI agent with the specific pitfalls to avoid before they attempt edits.

**Summary:** A high-density architectural document that explicitly foregrounds technical debt, type system conflicts, and build blockers.

**Source credibility:** Low; the repository lacks stars, description, and has not been updated in 7 months.

**Recency:** Current-era; utilizes modern Next.js 14 and TypeScript patterns.

**Source:** [K41R0N/Figaro-Design-Library/Claude.md](https://github.com/K41R0N/Figaro-Design-Library/blob/b86e43669a5a88a6de48dc51aaf41f64dd27c47a/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Component Sandbox - Architecture Documentation

## Project Purpose
A Next.js-based design system management application that allows users to:
- Create, edit, and organize UI components (HTML/CSS/JS)
- Preview components in isolated iframes
- Tag and categorize components by project
- Export/package selected components for reuse
- Mock authentication with GitHub/Google

## Tech Stack
- **Framework**: Next.js 14.1.0 (App Router)
- **Language**: TypeScript 5.4.2
- **UI Library**: Radix UI primitives
- **Styling**: TailwindCSS with custom design tokens (sage, terracotta colors)
- **Icons**: Lucide React
- **Deployment**: Netlify with @netlify/plugin-nextjs

## Application Structure

### Routes (Next.js App Router)
1. **`/` (app/page.tsx)** - Landing page
   - Marketing page with inline demo editor
   - Shows example component with live editing
   - Links to dashboard

2. **`/dashboard` (app/dashboard/page.tsx)** - Main application
   - Full CRUD for components
   - Project and tag management
   - Component preview and export functionality
   - Uses database-context for state management

### Key Components

#### State Management (lib/)
- **`auth-context.tsx`** - Mock authentication (l
```

</details>
