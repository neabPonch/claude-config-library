---
name: dilgerma__node-apps-with-eventsourcing-and-ralph-loop
source: https://github.com/dilgerma/node-apps-with-eventsourcing-and-ralph-loop/blob/170f5ad62dd361636d38a8eb567b4c442c22067d/Claude.md
repo: dilgerma/node-apps-with-eventsourcing-and-ralph-loop
kind: claude-md
stars: 7
last_pushed: 2026-03-05T15:18:34Z
license: unknown
score: 8
domains: [web-frontend, architecture]
tags: [domain-driven-design, strict-constraints, automated-testing]
curated: 2026-06-14
curated_by: config-scout
---

# dilgerma/node-apps-with-eventsourcing-and-ralph-loop — claude-md

**Why it's worth keeping:** It utilizes negative constraints (telling the AI what NOT to touch) and includes a powerful post-edit automation instruction to run tests automatically.

**Summary:** This configuration enforces a strict domain-driven 'slice' architecture with explicit boundaries on file access and modification.

**Source credibility:** Low star count, but the highly specific architectural rules suggest a functional project tool rather than a generic template.

**Recency:** Current; demonstrates high awareness of agentic workflows like auto-running tests after edits.

**Source:** [dilgerma/node-apps-with-eventsourcing-and-ralph-loop/Claude.md](https://github.com/dilgerma/node-apps-with-eventsourcing-and-ralph-loop/blob/170f5ad62dd361636d38a8eb567b4c442c22067d/Claude.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Configuration

Read Events in src/events to understand the global structure.

## Framework & Styling

- **CSS Framework**: Use Bulma CSS exclusively for all styling
- **Assumption**: Bulma CSS is already available and imported in the project
- **Styling Guidelines**:
    - Use Bulma's utility classes and components
    - Follow Bulma's naming conventions and class structure
    - Leverage Bulma's responsive design features
    - Prefer Bulma components over custom CSS

## File Structure Constraints

- **Strict Path Limitation**: if not instructed otherwise, only check `src/slices/{slicename}/*.ts`
- **Slice Organization**: Each feature/domain should be organized as a separate slice

## Code Standards

- **Language**: TypeScript only
- **Module System**: Use ES modules (import/export)
- **Type Safety**: Ensure all code is properly typed

## Development Guidelines

1. Each slice should be self-contained and focused on a specific domain
2. Use Bulma's grid system, components, and utilities for all UI-related code
3. Maintain clear separation of concerns within each slice
4. Follow TypeScript best practices for type definitions and interfaces

Only check src/slices/{slice}/*.
```

</details>
