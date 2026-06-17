---
name: dhes__cervical-cancer-cds
source: https://github.com/dhes/cervical-cancer-cds/blob/1d266db4d42ff3b7c35766981feb4fc93bf32783/CLAUDE.md
repo: dhes/cervical-cancer-cds
kind: claude-md
stars: 1
last_pushed: 2026-05-28T02:49:44Z
license: apache-2.0
score: 9
domains: [healthcare, fhir, documentation]
tags: [constraints, context-linking, build-guide]
curated: 2026-06-15
curated_by: config-scout
---

# dhes/cervical-cancer-cds — claude-md

**Why it's worth keeping:** Uses 'negative constraints' to prevent the AI from undoing intentional configuration choices and integrates local directory pointers for extended context.

**Summary:** Defines strict architectural constraints and provides detailed build instructions for a complex medical software project.

**Source credibility:** High-quality, specialized technical documentation from an active health-tech development process.

**Recency:** Current; utilizes modern Claude project-memory patterns.

**Source:** [dhes/cervical-cancer-cds/CLAUDE.md](https://github.com/dhes/cervical-cancer-cds/blob/1d266db4d42ff3b7c35766981feb4fc93bf32783/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Cervical Cancer Screening DAK (Working Draft)

## Status

**v2 scaffold-restart, in progress (2026-05).** v1 work — an OpenMRS-targeted CDS implementation with 5 CQL libraries, 4 PlanDefinitions, and 82/82 passing assertions — is preserved on the `v1-archive` branch (`git checkout v1-archive`). The `main` branch has been rescaffolded against the WHO `smart-dak-empty` template (CC BY 4.0) with Hopena Health identity and a non-endorsement disclaimer; v2 content authoring is the next phase.

This is an **unofficial**, in-progress draft. Not WHO-endorsed.

## Where the project context lives

Persistent project context (role framing, scope decisions, L4 direction, trajectory with WHO contacts, methodology references) is maintained in the user's Claude memory directory, not in this file:

```
~/.claude/projects/-Users-danheslinga-projects/memory/
```

See `MEMORY.md` in that directory for the index. Read those files at the start of any session involving this repo.

## v2 scope (first pass)

- **L1:** WHO cervical cancer screening guideline (2021 + updates), Algorithm 5 (HPV DNA + VIA triage), narrowed to **Eligibility Decision** and **Needs Screening Decision** only.
- **L2:** Minimal-
```

</details>
