---
name: Cindanela__svensk-kassa
source: https://github.com/Cindanela/svensk-kassa/blob/4257b8199a9b7355dc6da1daa67eb79710e78335/CLAUDE.MD
repo: Cindanela/svensk-kassa
kind: claude-md
stars: 0
last_pushed: 2026-01-07T11:59:28Z
license: unknown
score: 8
domains: [web-frontend]
tags: [nextjs, currency-app, state-management]
curated: 2026-06-16
curated_by: config-scout
---

# Cindanela/svensk-kassa — claude-md

**Why it's worth keeping:** Includes a highly valuable 'Known Gotchas' section to prevent common bugs and provides exact code snippets for critical patterns like currency formatting.

**Summary:** A comprehensive project guide that combines high-level architecture with specific implementation details for a Next.js application.

**Source credibility:** Low social proof (0 stars), but the content structure is professional-grade.

**Recency:** Very current, utilizing Next.js 15 and React 19 standards.

**Source:** [Cindanela/svensk-kassa/CLAUDE.MD](https://github.com/Cindanela/svensk-kassa/blob/4257b8199a9b7355dc6da1daa67eb79710e78335/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - Svensk Kassa

## Project Overview

Svensk Kassa is a Swedish cash register calculator application built with Next.js. It helps users count and calculate totals for Swedish currency (SEK) including coins and banknotes. The application provides a clean interface for counting denominations, tracking totals, and exporting/importing cash register data.

## Tech Stack

- **Framework**: Next.js 15.5.9 (with Turbopack)
- **React**: 19.2.1
- **TypeScript**: 5.x
- **Styling**: Tailwind CSS 3.4.1 + tailwindcss-animate
- **UI Components**: Radix UI (comprehensive component library)
- **Icons**: Lucide React
- **AI**: Google Genkit 1.20.0 (for AI features)
- **Backend**: Firebase 11.9.1
- **Form Handling**: React Hook Form 7.54.2 + Zod validation
- **Date Handling**: date-fns 3.6.0
- **Charts**: Recharts 2.15.1

## Project Structure

```
svensk-kassa/
├── src/
│   ├── app/
│   │   ├── page.tsx          # Main cash register interface
│   │   └── layout.tsx         # Root layout
│   ├── components/
│   │   ├── ui/                # Radix UI components (shadcn/ui style)
│   │   └── denomination-icon.tsx
│   ├── lib/
│   │   └── denominations.ts   # Swedish currency definitions
│   ├──
```

</details>
