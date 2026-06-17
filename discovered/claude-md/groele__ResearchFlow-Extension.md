---
name: groele__ResearchFlow-Extension
source: https://github.com/groele/ResearchFlow-Extension/blob/51c54302bc1193262c42f8c30f4fd1f6825fb3cb/claude.md
repo: groele/ResearchFlow-Extension
kind: claude-md
stars: 0
last_pushed: 2026-05-30T16:03:44Z
license: unknown
score: 8
domains: [web-frontend, chrome-extension]
tags: [react, wxt, typescript, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# groele/ResearchFlow-Extension — claude-md

**Why it's worth keeping:** It provides explicit mapping of core utilities (like ID generation and Zod schemas) to their exact file paths, preventing an agent from reinventing common patterns.

**Summary:** A highly structured project context for a React-based Chrome extension that maps specific business logic to the file system.

**Source credibility:** Single developer repository with low social proof but high-quality technical documentation.

**Recency:** Very current, utilizing cutting-edge versions like React 19 and TypeScript 5.9.

**Source:** [groele/ResearchFlow-Extension/claude.md](https://github.com/groele/ResearchFlow-Extension/blob/51c54302bc1193262c42f8c30f4fd1f6825fb3cb/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ScholarFlow - Project Context

## Goal
Academic research productivity Chrome extension for physics/materials-science workflows. Capture literature, manage projects, track submissions, and sync across private clouds.

## Tech Stack
- **Frontend**: React 19 + TypeScript 5.9 (strict mode)
- **Extension Framework**: WXT 0.20 (Chrome MV3)
- **Styling**: Tailwind CSS 3.4 + CSS custom properties (teal primary palette)
- **Database**: IndexedDB via Dexie 4.0 (8 tables: projects, researchRecords, manuscripts, submissions, tasks, researchAreas, evidence, schemaTemplates)
- **State**: dexie-react-hooks (reactive queries), Zustand (UI state)
- **Validation**: Zod 3.24 (entity schemas)
- **Icons**: lucide-react
- **Components**: class-variance-authority (CVA) for variant management
- **Package Manager**: npm
- **Test Framework**: Vitest 3.0

## Architecture
- **entrypoints/**: WXT entry points (background, content, popup, sidepanel, options)
- **src/ui/**: Design tokens, theme CSS, shared component library (primitives, layout, domain)
- **src/features/**: Feature modules (dashboard, projects, records, kanban, timeline, settings, capture, copilot)
- **src/hooks/**: Shared custom hooks
- **src/
```

</details>
