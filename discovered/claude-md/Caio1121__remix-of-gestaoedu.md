---
name: Caio1121__remix-of-gestaoedu
source: https://github.com/Caio1121/remix-of-gestaoedu/blob/910a6c73f58b60a8597c9a02da7dc894b20e59ea/CLAUDE.MD
repo: Caio1121/remix-of-gestaoedu
kind: claude-md
stars: 0
last_pushed: 2026-05-06T19:05:21Z
license: unknown
score: 8
domains: [web-frontend, fullstack, agentic-workflow]
tags: [react, supabase, workflow-management, self-correction]
curated: 2026-06-15
curated_by: config-scout
---

# Caio1121/remix-of-gestaoedu — claude-md

**Why it's worth keeping:** The 'Self-Improvement Loop' (updating lessons.md) and the mandatory 'Plan First' step (todo.md) are excellent transferable patterns for maintaining consistency in long sessions.

**Summary:** A highly structured guide that combines technical architecture with an agentic workflow involving task planning and a self-improvement loop.

**Source credibility:** Low star count suggests it is a personal/smaller project, but the documentation density is high.

**Recency:** Current; mentions modern versions of libraries like TanStack Query v5.

**Source:** [Caio1121/remix-of-gestaoedu/CLAUDE.MD](https://github.com/Caio1121/remix-of-gestaoedu/blob/910a6c73f58b60a8597c9a02da7dc894b20e59ea/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Agent System Prompt

## Project Context
**EduFlow** — Plataforma SaaS de gestão educacional para alunos, professores e gestores.

- **Stack**: React 18, TypeScript, Vite, Tailwind CSS, shadcn/ui.
- **Backend**: Supabase (Auth + Postgres + Storage + Edge Functions).
- **State Management**: TanStack Query v5.
- **Testing**: Vitest.
- **Hooks Architecture**: Domain-separated (ver `src/hooks/`).

---

## Commands
- **Dev**: `npm run dev`
- **Build**: `npm run build`
- **Test single**: `npm run test -- src/test/example.test.ts`
- **Test all**: `npm run test`
- **Lint**: `npm run lint`
- **Type check**: `npm run build` (tsc via vite build)

---

## Architecture
- `src/hooks/` → Domain hooks (useProfile, useTeacherData, etc.)
- `src/components/teacher/` → TeacherClasses, ClassCard, CreateClassModal
- `src/components/student/` → Student panel components
- `src/components/manager/` → Manager panel components
- `src/pages/` → One page per role dashboard + auth pages
- `src/contexts/` → AuthContext (auth state + role detection)
- `src/types/index.ts` → Shared domain types
- `src/integrations/supabase/client.ts` → Supabase client instance
- `supabase/functions/` → Edge Functions
```

</details>
