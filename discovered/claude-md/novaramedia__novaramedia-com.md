---
name: novaramedia__novaramedia-com
source: https://github.com/novaramedia/novaramedia-com/blob/510598fe34e2c17cb72db4252b84b93be5b2944f/CLAUDE.md
repo: novaramedia/novaramedia-com
kind: claude-md
stars: 5
last_pushed: 2026-06-12T21:50:11Z
license: apache-2.0
score: 7
domains: [web-frontend, wordpress]
tags: [build-constraints, documentation-mapping, guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# novaramedia/novaramedia-com — claude-md

**Why it's worth keeping:** Uses 'Non-negotiable rules' to prevent automated breakage of the build system and maps out essential documentation directories for context injection.

**Summary:** Establishes strict build-system guardrails and provides a high-level map of project documentation and external task tracking.

**Source credibility:** Professional repository with active maintenance and cross-project shared conventions.

**Recency:** Current; utilizes modern development tooling like Webpack and Cypress.

**Source:** [novaramedia/novaramedia-com/CLAUDE.md](https://github.com/novaramedia/novaramedia-com/blob/510598fe34e2c17cb72db4252b84b93be5b2944f/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

WordPress theme for novaramedia.com. PHP + modular JS (Webpack) + Stylus (nm-stylus-library).

## Non-negotiable rules

- **Production-quality code only** — no experimental outputs
- **Don't modify build system** — Webpack/release config requires team approval
- **`dist/` commits** — only when source files actually changed (`npm run build` to verify)

## References

- GitHub: [novaramedia/novaramedia-com](https://github.com/novaramedia/novaramedia-com) — branch: `development`, PR target: `development`
- Notion project: search Novara workspace for `novaramedia-com` to find current version record (new record created each minor release)
- Code standards: `.github/copilot-instructions.md`
- Cross-project conventions: `nm-agents-shared/conventions.md`

## Docs

- `docs/architecture/` — block rendering, oEmbed privacy
- `docs/plans/` — embed consent gate, multi-newsletter signup, CI speedup
- `docs/specs/` — latest articles news category
- `docs/testing/` — Cypress testing, workflow notes, testing overview
- `docs/security.md` — security notes
- `docs/extended-changelogs/` — verbose PR changelogs
```

</details>
