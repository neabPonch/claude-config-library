---
name: PaulBratslavsky__astro-strapi-example-project
source: https://github.com/PaulBratslavsky/astro-strapi-example-project/blob/42a91ba42dbc7fd7196a8daf1230017f9f13406a/CLAUDE.md
repo: PaulBratslavsky/astro-strapi-example-project
kind: claude-md
stars: 96
last_pushed: 2026-04-08T01:10:49Z
license: unknown
score: 9
domains: [web-frontend, backend-api, cms]
tags: [astro, strapi, tailwind-v4, design-tokens, data-fetching]
curated: 2026-06-16
curated_by: config-scout
---

# PaulBratslavsky/astro-strapi-example-project — claude-md

**Why it's worth keeping:** The semantic design token table prevents 'hallucinated' styling, and the strict data-fetching (populate) constraints ensure efficient API usage. It also leverages custom skill patterns like '/add-page' to guide agent workflows.

**Summary:** A high-density instruction file that bridges design systems with technical implementation rules for Astro and Strapi.

**Source credibility:** Reliable example project with recent maintenance (2 months ago).

**Recency:** Highly current; uses cutting-edge tech like Tailwind v4 and Strapi 5.

**Source:** [PaulBratslavsky/astro-strapi-example-project/CLAUDE.md](https://github.com/PaulBratslavsky/astro-strapi-example-project/blob/42a91ba42dbc7fd7196a8daf1230017f9f13406a/CLAUDE.md) · 96★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Guidelines

## Stack

- **Frontend:** Astro 6 with Tailwind CSS v4
- **Backend:** Strapi 5 (latest) with SQLite
- **Content loader:** `strapi-community-astro-loader` v4 via Astro's Content Layer API
- **Package manager:** yarn

## UI and Design Preferences

### Design Tokens

This project uses a custom Tailwind v4 theme defined in `client/src/styles/global.css`. Always use semantic tokens — never raw Tailwind colors.

| Token | Purpose |
|---|---|
| `text-secondary` | Headings, primary text |
| `text-muted` | Body text, descriptions |
| `text-faint` | Metadata, captions |
| `text-primary-600` | Accent text, links, labels |
| `bg-surface` | Page background |
| `bg-surface-alt` | Alternate section backgrounds |
| `bg-surface-raised` | Cards, elevated elements |
| `border-border` / `border-border-hover` | Borders and hover states |
| `font-heading` | Heading font family |
| `rounded-xl` | Card corners |

### Design Principles

- **Content-appropriate layouts** — different content types should have different UI patterns. A team page should not look like a blog page. Match the layout to how users expect to see that type of content.
- **Visual hierarchy** — the most important f
```

</details>
