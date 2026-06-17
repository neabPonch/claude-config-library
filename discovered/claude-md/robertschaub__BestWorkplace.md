---
name: robertschaub__BestWorkplace
source: https://github.com/robertschaub/BestWorkplace/blob/a725bac787b0b323d0ffc1036590cf7d4ff7f6e7/CLAUDE.md
repo: robertschaub/BestWorkplace
kind: claude-md
stars: 0
last_pushed: 2026-02-21T18:13:07Z
license: other
score: 7
domains: [documentation, devops]
tags: [deployment-guardrails, role-based, tool-handoff]
curated: 2026-06-15
curated_by: config-scout
---

# robertschaub/BestWorkplace — claude-md

**Why it's worth keeping:** Provides excellent guardrails against breaking CI/CD pipelines and includes a sophisticated 'Agent Handoff' protocol for tool-switching context.

**Summary:** A workflow-centric guide for a documentation project that translates xWiki content to GitHub Pages.

**Source credibility:** Low star count, but the structure suggests a highly intentional orchestration of roles and tools.

**Recency:** Updated 4 months ago; aligns well with current agentic workflow practices.

**Source:** [robertschaub/BestWorkplace/CLAUDE.md](https://github.com/robertschaub/BestWorkplace/blob/a725bac787b0b323d0ffc1036590cf7d4ff7f6e7/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code instructions — BestWorkplace

Project rules and workflow: @AGENTS.md

## Project overview

Documentation-only project — no source code. xWiki 2.1 pages about agile leadership, team culture, and workplace transformation, published via GitHub Pages.

- `Docs/xwiki-pages/The Best Workplace/` — xWiki content pages (single source of truth)
- `Docs/xwiki-pages/scripts/` — Python build scripts and PowerShell deployment
- `Docs/xwiki-pages/viewer-impl/` — HTML viewer for local preview
- `Docs/xwiki-export/` — XAR snapshot files
- `.github/workflows/deploy-docs.yml` — CI/CD for gh-pages deployment

## Commands

- Preview: `Docs\xwiki-pages\View.cmd`
- Build gh-pages locally: `python Docs/xwiki-pages/scripts/build_ghpages.py`
- XAR → tree: `python Docs/xwiki-pages/scripts/xar_to_xwiki_tree.py <file.xar> --output Docs/xwiki-pages`
- Tree → XAR: `python Docs/xwiki-pages/scripts/xwiki_tree_to_xar.py Docs/xwiki-pages --output BestWorkplace.xar`
- Platform: Windows. Use PowerShell-compatible commands.

## Publishing (gh-pages)

**CI owns gh-pages. Agents must NEVER push to the gh-pages branch directly.**

- To publish: `git push` to `main` — CI (`.github/workflows/deploy-docs.yml`)
```

</details>
