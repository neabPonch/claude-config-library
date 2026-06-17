---
name: adnansadar__portfolio
source: https://github.com/adnansadar/portfolio/blob/86bd6b0086af1f140735d33329207fc6f13ff97d/CLAUDE.md
repo: adnansadar/portfolio
kind: claude-md
stars: 0
last_pushed: 2026-02-07T10:07:59Z
license: unknown
score: 7
domains: [web-frontend, nextjs]
tags: [react, typescript, tailwind, shadcn]
curated: 2026-06-14
curated_by: config-scout
---

# adnansadar/portfolio — claude-md

**Why it's worth keeping:** The mandated 'build then format' sequence creates a reliable self-correction cycle for agents, while specific utility instructions (like the `cn()` pattern) prevent common styling errors.

**Summary:** Defines a strict build-and-format verification loop and clear component implementation standards for a shadcn/ui stack.

**Source credibility:** Low; individual portfolio project with no social proof or history.

**Recency:** Current; follows modern React/Next.js development patterns.

**Source:** [adnansadar/portfolio/CLAUDE.md](https://github.com/adnansadar/portfolio/blob/86bd6b0086af1f140735d33329207fc6f13ff97d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Guidelines for Portfolio Project

## Development Workflow

### Code Formatting

After making any code changes, always run the following commands in sequence:

1. **Build the project** to verify no errors:

   ```bash
   npm run build
   ```

2. **Format the codebase** with Prettier:
   ```bash
   npx prettier --write "src/**/*.{js,jsx,ts,tsx,json,css,md}"
   ```

This ensures:

- All code changes are validated before formatting
- Consistent code style across the entire codebase
- No formatting issues in committed code

## Project Standards

### Tech Stack

- **Framework**: Next.js 16.1.2 with Turbopack
- **Language**: TypeScript
- **Styling**: Tailwind CSS with shadcn/ui components
- **Animations**: Framer Motion

### Code Style

- Follow the Prettier configuration in `.prettierrc`
- Use the shadcn/ui design system for components
- Leverage design tokens from `src/design-system`
- Use TypeScript for all components (no `.jsx` files)

### Component Patterns

- All components should be TypeScript React components
- Use the `cn()` utility from `@/lib/utils` for conditional class names
- Import design system utilities from `@/design-system`
- Use shadcn/ui components inste
```

</details>
