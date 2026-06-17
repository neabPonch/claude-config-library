---
name: danyelajunebrown__Reparations-is-a-real-number
source: https://github.com/danyelajunebrown/Reparations-is-a-real-number/blob/ae15828fd0019f37bedae3cc55124e8206831923/Claude.md
repo: danyelajunebrown/Reparations-is-a-real-number
kind: claude-md
stars: 0
last_pushed: 2026-06-13T01:15:16Z
license: unknown
score: 9
domains: [data-engineering, web-scraping, backend-api]
tags: [data-integrity, automation-traps, schema-management, provenance]
curated: 2026-06-14
curated_by: config-scout
---

# danyelajunebrown/Reparations-is-a-real-number — claude-md

**Why it's worth keeping:** Highlights specific 'traps' regarding DB driver quirks, JSONB encoding issues, and scraper-specific environment constraints that prevent common automation failures.

**Summary:** Defines strict data provenance and integrity protocols for a complex genealogical database involving high-stakes legal instruments.

**Source credibility:** High technical density despite low social proof/stars; demonstrates deep domain knowledge of data edge cases.

**Recency:** Current; includes modern cloud-database and headless-browser specific behaviors.

**Source:** [danyelajunebrown/Reparations-is-a-real-number/Claude.md](https://github.com/danyelajunebrown/Reparations-is-a-real-number/blob/ae15828fd0019f37bedae3cc55124e8206831923/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

> Loaded at the start of every session. Keep under 220 lines. Prune ruthlessly when adding.
> Last reviewed: 2026-05-25.

## What this project actually is

An aggregated database of digitized slavery records, indexed to **enslaved persons**, **enslavers**, and **opted-in descendants of both classes**. The output that justifies the work is the **Debt Acknowledgment Agreement (DAA)** — a generated, signed legal instrument that names every documented slaveholder ancestor of a descendant and every documented enslaved person owned, with primary-source citations (FamilySearch ARKs, MSA certificates, civilwardc petitions, etc.), and that grounds annual government petitions under an Article V framework. DAAs are settled via the `ReparationsEscrow` contract on Base mainnet.

The README at repo root is out of date and describes an older “document upload pipeline” scope. The scope above is canonical.

## Audit-grade rules (non-negotiable)

1. **No model output gets aggregated, totaled, or summed.** The model orchestrates; deterministic code computes; humans review. Any number that appears on a DAA must trace to a row, a citation, and a methodology version.
1. **Every external cla
```

</details>
