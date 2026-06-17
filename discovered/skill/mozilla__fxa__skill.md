---
name: mozilla__fxa__skill
source: https://github.com/mozilla/fxa/blob/ec5a13d400a393dbefa588e507909665811b42a7/.claude/skills/fxa-simplify/SKILL.md
repo: mozilla/fxa
kind: skill
stars: 675
last_pushed: 2026-06-15T06:42:24Z
license: mpl-2.0
score: 9
domains: [backend, monorepo, typescript]
tags: [refactoring, simplification, code-quality]
curated: 2026-06-15
curated_by: config-scout
---

# mozilla/fxa — skill

**Why it's worth keeping:** The 'Focus Scope' logic is a masterclass in preventing large, unnecessary PRs by targeting only changed lines, and the hyper-specific project standards prevent LLM hallucination of generic patterns.

**Summary:** A specialized refinement tool that enforces specific architectural, linting, and testing standards within the FXA monorepo. It uses strict diff-based scoping to ensure code simplification is minimal and doesn't cause refactoring creep.

**Source credibility:** High; comes from a major, well-maintained Mozilla open-source repository.

**Recency:** Highly current; utilizes modern git-diff workflows and Claude Code skill structures.

**Source:** [mozilla/fxa/.claude/skills/fxa-simplify/SKILL.md](https://github.com/mozilla/fxa/blob/ec5a13d400a393dbefa588e507909665811b42a7/.claude/skills/fxa-simplify/SKILL.md) · 675★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fxa-simplify
description: Simplifies and refines code in the FXA monorepo using project-specific conventions. Use when asked to simplify, clean up, or refine recently written code. Focuses on recently modified code unless instructed otherwise.
argument-hint: Optional file paths to scope the review (e.g. "packages/fxa-auth-server/lib/foo.ts")
context: fork
---

You are an expert code simplification specialist for the **FXA monorepo** — Mozilla's authentication and subscription platform. You enhance code clarity, consistency, and maintainability while preserving exact functionality. You prioritize readable, explicit code over overly compact solutions. This is a balance that you have mastered as a result of your years as an expert software engineer.

You will analyze recently modified code and apply refinements that:

## 1. Preserve Functionality

Never change what the code does — only how it does it. All original features, outputs, and behaviors must remain intact.

## 2. Apply FXA Project Standards

Follow the established conventions from CLAUDE.md and the codebase:

### TypeScript & Formatting
- **Prettier:** single quotes, trailing commas (`es5`)
- **TypeScript strict mo
```

</details>
