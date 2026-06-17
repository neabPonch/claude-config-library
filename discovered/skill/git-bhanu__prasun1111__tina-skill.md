---
name: git-bhanu__prasun1111__tina-skill
source: https://github.com/git-bhanu/prasun1111/blob/86c27604f48fb44d9dc40ba15e00bcccd561a397/docs/tina-skill.md
repo: git-bhanu/prasun1111
kind: skill
stars: 0
last_pushed: 2026-06-15T07:38:50Z
license: apache-2.0
score: 8
domains: [web-frontend, cms]
tags: [tinacms, nextjs, visual-editing]
curated: 2026-06-16
curated_by: config-scout
---

# git-bhanu/prasun1111 — skill

**Why it's worth keeping:** It defines the exact server/client component split required for visual editing and provides strict 'anti-patterns' to prevent broken click-to-edit functionality.

**Summary:** Provides highly specific implementation rules for integrating TinaCMS with Next.js App Router, focusing on visual editing and data fetching patterns.

**Source credibility:** The source is a low-reputation personal repository, likely containing project-specific documentation.

**Recency:** Current, utilizing modern Next.js App Router and TinaCMS paradigms.

**Source:** [git-bhanu/prasun1111/docs/tina-skill.md](https://github.com/git-bhanu/prasun1111/blob/86c27604f48fb44d9dc40ba15e00bcccd561a397/docs/tina-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TinaCMS Skill

Use this guide when implementing or modifying TinaCMS-backed features in this repository.

## Goal
- Keep Tina changes schema-driven, strongly typed, and compatible with the existing Next.js App Router plus Tina visual editing flow.

## Repository-Specific Rules
- Fetch content on the server with `client.queries.*()`.
- When a route supports visual editing, keep the server/client split:
  - `page.tsx` fetches data.
  - `client-page.tsx` calls `useTina({ query, data, variables })`.
- Always pass all three Tina values to the client component: `query`, `data`, and `variables`.
- For visual editing, prefer querying an individual document for the editable page state.
- Import generated Tina query types from `@/tina/__generated__/types`.
- Prefer content-driven changes in `content/` over hardcoding editable strings in JSX.
- Keep schema and rendering in sync. If you add or rename fields in `tina/`, update the UI that renders them.
- Use `data-tina-field={tinaField(object, 'fieldName')}` only on visible editable elements.
- Pass the source object to `tinaField()`, not a derived primitive.
- Prefer existing collections, templates, and field helpers before adding new abstra
```

</details>
