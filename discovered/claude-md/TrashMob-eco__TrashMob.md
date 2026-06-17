---
name: TrashMob-eco__TrashMob
source: https://github.com/TrashMob-eco/TrashMob/blob/569b59934dd2ed652fdd05dee6c194cf6f03f290/CLAUDE.md
repo: TrashMob-eco/TrashMob
kind: claude-md
stars: 18
last_pushed: 2026-06-15T00:47:09Z
license: apache-2.0
score: 9
domains: [backend-api, web-frontend, .net-stack, fullstack]
tags: [architecture-patterns, coding-standards, ai-instructions, dotnet]
curated: 2026-06-15
curated_by: config-scout
---

# TrashMob-eco/TrashMob — claude-md

**Why it's worth keeping:** Includes a critical 'AI Assistant Boundaries' section to prevent autonomous structural changes and provides highly specific C# conventions that mitigate common library-specific bugs (like EF Core null check edge cases).

**Summary:** A comprehensive guide covering build processes, architectural patterns, domain logic, and environment setup. It includes explicit instructions for AI behavior boundaries and granular coding standards.

**Source credibility:** High-quality documentation from an active project with professional-grade architecture.

**Recency:** Extremely current, leveraging cutting-edge technologies like .NET 10 and Vite 7.

**Source:** [TrashMob-eco/TrashMob/CLAUDE.md](https://github.com/TrashMob-eco/TrashMob/blob/569b59934dd2ed652fdd05dee6c194cf6f03f290/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Run Commands

### Backend (.NET 10)
```bash
dotnet build                              # Build solution
dotnet run --environment Development      # Run web API (from TrashMob/ folder)
dotnet test                               # Run tests (from TrashMob.Shared.Tests/)
```

### Frontend (React/Vite)
```bash
cd TrashMob/client-app
npm install        # Install dependencies
npm start          # Dev server
npm run build      # Production build
npm test           # Run Vitest tests
npm run lint       # ESLint with fixes
npm run format     # Prettier formatting
npm run check      # Both lint + format (matches CI)
```

### E2E Tests (Playwright)
```bash
cd TrashMob/client-app
npm run e2e                           # Run all E2E tests (197 tests)
npm run e2e -- --project=chromium     # Chromium only
npm run e2e -- --grep "Dashboard"     # Filter by name
BASE_URL=https://dev.trashmob.eco npm run e2e  # Against deployed dev
```

### Database Migrations
```bash
# From TrashMob folder
dotnet ef migrations add <MigrationName>
dotnet ef database update
```

## Architectur
```

</details>
