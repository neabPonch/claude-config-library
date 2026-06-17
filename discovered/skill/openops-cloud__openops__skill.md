---
name: openops-cloud__openops__skill
source: https://github.com/openops-cloud/openops/blob/8072ed243963963eb1e91955d2c0e713c468b4cf/.claude/skills/react/SKILL.md
repo: openops-cloud/openops
kind: skill
stars: 1034
last_pushed: 2026-06-15T09:58:45Z
license: other
score: 9
domains: [web-frontend, react]
tags: [react, ui-ux, performance, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# openops-cloud/openops — skill

**Why it's worth keeping:** It includes actionable anti-pattern checklists (e.g., inline object literals) and a unique 'overflow behavior' protocol to prevent common UI regressions in agentic workflows. The instructions on referential stability and query key management are highly transferable for any complex React project.

**Summary:** A highly specific technical specification for frontend engineering that enforces architectural boundaries, performance optimization, and UI stability.

**Source credibility:** High; the source repository is a well-starred, actively maintained open-source platform.

**Recency:** 

**Source:** [openops-cloud/openops/.claude/skills/react/SKILL.md](https://github.com/openops-cloud/openops/blob/8072ed243963963eb1e91955d2c0e713c468b4cf/.claude/skills/react/SKILL.md) · 1034★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: react
description: >
  Use when creating or editing frontend React code in react-ui or ui-components packages.
  Triggers on any frontend component, hook, or UI work.
---

# React & Frontend Development Skill

When working on frontend code in `packages/react-ui` or `packages/ui-components`, follow these guidelines strictly.

---

## 1. Modular Components

- Break the design into independent files. Avoid large, single-file outputs.
- Each component should have one clear responsibility.
- Reusable, pure components live in `packages/ui-components` and **must** have Storybook stories in `packages/ui-components/src/stories/`.
- Application-specific components live in `packages/react-ui`.
- Do not make breaking changes to existing component interfaces (props, names) without discussion.

---

## 2. Logic Isolation

- Move event handlers and business logic into **custom hooks** (`use-*.ts`).
- Follow existing convention: hooks go in `hooks/` directories alongside features (e.g., `features/campaigns/hooks/use-campaign-charts.ts`).
- Keep component files focused on rendering; delegate logic to hooks.
- Extract complex derived state into hooks or utility functions.

---

## 3. Data
```

</details>
