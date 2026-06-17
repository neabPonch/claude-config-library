---
name: GerritCodeReview__gerrit__skill
source: https://github.com/GerritCodeReview/gerrit/blob/3972032bd848117f5e59491b09ca14f21fca84e9/configs/skills/gerrit_frontend_engineering/SKILL.md
repo: GerritCodeReview/gerrit
kind: skill
stars: 1189
last_pushed: 2026-06-14T09:17:19Z
license: apache-2.0
score: 9
domains: [web-frontend, architecture, typescript]
tags: [lit, ui-standards, engineering-guides]
curated: 2026-06-15
curated_by: config-scout
---

# GerritCodeReview/gerrit — skill

**Why it's worth keeping:** The 'Symptom/Trap' mapping provides specific failure modes that allow an AI agent to understand not just what to do, but exactly which regressions to avoid.

**Summary:** A high-density engineering standard for frontend architecture using the Lit framework and TypeScript.

**Source credibility:** Extremely high; sourced from Gerrit, a major industrial-scale open-source project.

**Recency:** Current; includes modern concerns like AI context optimization and telemetry.

**Source:** [GerritCodeReview/gerrit/configs/skills/gerrit_frontend_engineering/SKILL.md](https://github.com/GerritCodeReview/gerrit/blob/3972032bd848117f5e59491b09ca14f21fca84e9/configs/skills/gerrit_frontend_engineering/SKILL.md) · 1189★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gerrit-frontend-engineering
description: Provides guidance and best practices on Polygerrit UI development, frontend architecture, and TypeScript/JS coding standards in Gerrit.
---

# Frontend Engineering & UI Development Engineering Guide

## Executive Summary

Welcome to the Frontend Engineering & UI Development guide. This repository
serves as the authoritative source of tribal knowledge for our UI architecture,
born from historical refactoring efforts, critical performance optimizations,
and the ongoing necessity to prevent recurrent regression of known failure
modes. By codifying these engineering standards, we ensure that incoming
engineers can confidently navigate the complexities of our frontend ecosystem
without falling into legacy traps, introducing unverified UI states, or
triggering silent runtime failures.

This guide enforces strict architectural boundaries across the entire UI
development lifecycle. It mandates rigorous state encapsulation within the Lit
framework, uncompromising TypeScript type safety, and highly resilient
client-server integrations. It further standardizes hermetic UI testing
methodologies, unifies our CSS design systems, and outlines str
```

</details>
