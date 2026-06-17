---
name: alekspetrov__navigator__task-17-visual-regression-skill
source: https://github.com/alekspetrov/navigator/blob/d52c41f957afe1a0b54ebd0abae9360101dd8225/.agent/tasks/archive/TASK-17-visual-regression-skill.md
repo: alekspetrov/navigator
kind: skill
stars: 191
last_pushed: 2026-06-15T10:00:58Z
license: unknown
score: 8
domains: [web-frontend, devops, automation]
tags: [visual-regression, storybook, chromatic, ci-cd, skill-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# alekspetrov/navigator — skill

**Why it's worth keeping:** Uses a highly structured architectural blueprint with granular function signatures (detect -> analyze -> generate) and Jinja2 templates to ensure repeatable, production-ready automation.

**Summary:** Automates the full lifecycle of visual regression testing by generating Storybook stories, tool configurations, and CI/CD workflows from component analysis.

**Source credibility:** High; the source repository is an established project focused on advanced context engineering.

**Recency:** Very current, utilizing modern tools like Chromatic and recent GitHub Actions patterns.

**Source:** [alekspetrov/navigator/.agent/tasks/archive/TASK-17-visual-regression-skill.md](https://github.com/alekspetrov/navigator/blob/d52c41f957afe1a0b54ebd0abae9360101dd8225/.agent/tasks/archive/TASK-17-visual-regression-skill.md) · 191★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TASK-17: Visual Regression Integration Skill

**Status**: 🚧 In Progress
**Priority**: High
**Complexity**: Medium
**Version**: v3.3.0
**Created**: 2025-10-21

---

## 🎯 Objective

Create `visual-regression` skill to automate visual regression testing setup with Chromatic, Percy, or BackstopJS integration.

**User value**: Reduce visual regression setup from 2-3 hours to 5 minutes, ensure pixel-perfect implementation of designs, prevent design system drift.

---

## 📋 Context

Navigator v3.2 introduced `product-design` skill for Figma design handoff. Visual regression closes the loop:

```
Design (Figma) → Code (product-design) → Validation (visual-regression) → CI/CD
```

**Problem**: Setting up visual regression requires:
- Storybook configuration
- Test tool setup (Chromatic/Percy/BackstopJS)
- Story file generation
- CI/CD integration
- Design token validation

**Solution**: Auto-generate all configuration, stories, and CI workflows.

---

## 🏗️ Architecture

### Skill Structure

```
skills/visual-regression/
├── SKILL.md                          # Auto-invocation, instructions
├── functions/
│   ├── story_generator.py            # Generate Storybook stories
│   ├── chromatic_
```

</details>
