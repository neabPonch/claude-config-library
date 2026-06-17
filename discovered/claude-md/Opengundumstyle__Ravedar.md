---
name: Opengundumstyle__Ravedar
source: https://github.com/Opengundumstyle/Ravedar/blob/d1f048b9c59d8cd6f9150b2fc6a9568585dbd847/CLAUDE.md
repo: Opengundumstyle/Ravedar
kind: claude-md
stars: 0
last_pushed: 2026-06-05T18:12:57Z
license: unknown
score: 9
domains: [web-frontend, design-systems]
tags: [nextjs, ui-ux, css-tokens]
curated: 2026-06-16
curated_by: config-scout
---

# Opengundumstyle/Ravedar — claude-md

**Why it's worth keeping:** The use of a custom `rd-*` namespace to guard visual identity and the inclusion of a practical UI checklist for PRs are elite techniques. It also documents 'lessons learned' regarding technical pitfalls like pointer-events.

**Summary:** Enforces a strict, opinionated design system to prevent generic 'AI mockup' aesthetics through a custom CSS namespace. It includes specific component assembly patterns and typography rules.

**Source credibility:** Low social proof/stars, but the high density of specific design tokens suggests a highly organized personal project.

**Recency:** Very current; references Next.js 14 App Router and modern React patterns.

**Source:** [Opengundumstyle/Ravedar/CLAUDE.md](https://github.com/Opengundumstyle/Ravedar/blob/d1f048b9c59d8cd6f9150b2fc6a9568585dbd847/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RAVEDAR — Project Guide for Claude

## Project at a glance

Ravedar is a Next.js 14 (App Router) app for matching people attending the same rave / festival. Auth via Supabase. Real users live alongside seeded "demo" profiles. Visual identity is **graffiti-meets-rave-warehouse**: spray-painted neon over concrete walls.

---

## UI methodology — cohesive look across all pages

The look is enforced by a single design system in `app/globals.css` (the `rd-*` namespace) plus shared React components in `app/components/`. **All new pages MUST consume this system instead of inventing one-off Tailwind chains.** Generic indigo→purple→pink gradients (`bg-gradient-to-br from-indigo-900 via-purple-900 to-pink-900`) are forbidden — that's the "default AI mockup" look and it clashes with the rest of the app.

### 1. Design tokens (defined in `:root` in `globals.css`)

**Spray-paint accents** — neon, used for highlights, focus, active state:
- `--rd-spray-pink: #ff1a8a` — primary accent (hover, active, brand)
- `--rd-spray-yellow: #ffe900` — "hot" / featured emphasis (e.g. trending city, sticker)
- `--rd-spray-cyan: #00e7ff` — neon button glow, radar
- `--rd-spray-green: #66ff00` — live/success/o
```

</details>
