---
name: dkyazzentwatwa__SuperNavigator__task-17-visual-regression-skill
source: https://github.com/dkyazzentwatwa/SuperNavigator/blob/a8851214e716eec4dcbd22df489bff7bd7e87e06/.agent/tasks/TASK-17-visual-regression-skill.md
repo: dkyazzentwatwa/SuperNavigator
kind: skill
stars: 32
last_pushed: 2026-01-23T03:34:30Z
license: other
score: 8
domains: [web-frontend, devops, testing, automation]
tags: [visual-regression, storybook, chromatic, ci-cd, automation-blueprint]
curated: 2026-06-15
curated_by: config-scout
---

# dkyazzentwatwa/SuperNavigator — skill

**Why it's worth keeping:** It utilizes a 'detection-first' architecture to validate existing environments before acting and provides highly structured logic for component analysis and CI/CD generation.

**Summary:** A comprehensive technical blueprint for automating visual regression testing integration via Storybook and Chromatic.

**Source credibility:** Moderate popularity (32 stars) from a specialized repository focused on agentic navigation.

**Recency:** Current; uses modern standards like TypeScript, GitHub Actions, and recent Storybook patterns.

**Source:** [dkyazzentwatwa/SuperNavigator/.agent/tasks/TASK-17-visual-regression-skill.md](https://github.com/dkyazzentwatwa/SuperNavigator/blob/a8851214e716eec4dcbd22df489bff7bd7e87e06/.agent/tasks/TASK-17-visual-regression-skill.md) · 32★

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
