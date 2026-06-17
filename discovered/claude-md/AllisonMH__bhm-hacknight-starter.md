---
name: AllisonMH__bhm-hacknight-starter
source: https://github.com/AllisonMH/bhm-hacknight-starter/blob/7407b0c69c355dae9994fc77ac0c14e2a12f2a41/CLAUDE.md
repo: AllisonMH/bhm-hacknight-starter
kind: claude-md
stars: 0
last_pushed: 2026-02-15T20:02:00Z
license: unknown
score: 8
domains: [web-frontend, design-systems]
tags: [react, scss, bem, instructional-pitfalls]
curated: 2026-06-15
curated_by: config-scout
---

# AllisonMH/bhm-hacknight-starter — claude-md

**Why it's worth keeping:** The 'Common Pitfalls' table is an elite technique for providing negative constraints, while the explicit design system rules (BEM/nesting limits) ensure visual consistency.

**Summary:** A highly detailed instruction set that defines not just the 'what' but the 'how' of coding and styling. It uses a specific pitfalls table to prevent AI-driven architectural drift.

**Source credibility:** Personal project starter; high quality in documentation despite low social proof.

**Recency:** Very current; reflects modern web development workflows and LLM interaction patterns.

**Source:** [AllisonMH/bhm-hacknight-starter/CLAUDE.md](https://github.com/AllisonMH/bhm-hacknight-starter/blob/7407b0c69c355dae9994fc77ac0c14e2a12f2a41/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

**bhm-hacknight-starter** is a React single-page application that presents chronologically ordered mini biographies of Black History major figures and their contributions. It is built with React, Vite, and SCSS, and deployed to Vercel.

## Repository Structure

```
bhm-hacknight-starter/
├── index.html                    # HTML entry point
├── package.json                  # Dependencies and scripts
├── vite.config.js                # Vite configuration
├── vercel.json                   # Vercel deployment config
├── src/
│   ├── main.jsx                  # React entry point
│   ├── App.jsx                   # Root component
│   ├── components/
│   │   ├── Header.jsx            # Page header with title
│   │   ├── Timeline.jsx          # Timeline layout, loads and sorts biographies
│   │   ├── BiographyCard.jsx     # Individual biography card
│   │   └── Footer.jsx            # Page footer
│   ├── data/
│   │   └── biographies.json      # All biography entries (sorted by sortYear)
│   └── scss/
│       ├── _variables.scss       # Colors, spacing, breakpoints
│       └── styles.scss           # All component styles (BEM naming)
├── README.md
└── CLA
```

</details>
