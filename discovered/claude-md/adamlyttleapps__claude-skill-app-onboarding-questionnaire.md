---
name: adamlyttleapps__claude-skill-app-onboarding-questionnaire
source: https://github.com/adamlyttleapps/claude-skill-app-onboarding-questionnaire/blob/5bc4786d80f2c23de60b3ba02773e919ed8fd091/CLAUDE.md
repo: adamlyttleapps/claude-skill-app-onboarding-questionnaire
kind: claude-md
stars: 1064
last_pushed: 2026-04-06T11:04:41Z
license: mit
score: 9
domains: [ai-agents, mobile-ux, growth-engineering]
tags: [onboarding-flow, conversion-psychology]
curated: 2026-06-15
curated_by: config-scout
---

# adamlyttleapps/claude-skill-app-onboarding-questionnaire — claude-md

**Why it's worth keeping:** It demonstrates how to embed complex domain logic (a 14-step conversion framework) into project instructions to ensure the agent acts as a subject matter expert rather than a generalist.

**Summary:** Defines the architectural and psychological blueprint for a specialized Claude Code skill that generates high-conversion mobile onboarding flows.

**Source credibility:** High; significant star count and highly specialized niche.

**Recency:** Current; explicitly leverages Claude Code's specific memory and skill capabilities.

**Source:** [adamlyttleapps/claude-skill-app-onboarding-questionnaire/CLAUDE.md](https://github.com/adamlyttleapps/claude-skill-app-onboarding-questionnaire/blob/5bc4786d80f2c23de60b3ba02773e919ed8fd091/CLAUDE.md) · 1064★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A Claude Code skill (`app-onboarding-questionnaire`) that designs and builds high-converting questionnaire-style onboarding flows for any app. Modelled on proven conversion patterns from top subscription apps (Mob, Headspace, Noom, Duolingo). Invoked via `/app-onboarding-questionnaire` from within a user's app project.

## Skill Structure

- **SKILL.md** — The skill prompt. Defines a 5-phase workflow: App Discovery → User Transformation → Blueprint → Screen Content → Implementation. Uses memory to persist state across conversations.
- **CLAUDE.md** — This file. Development guidance for working on the skill itself.

## The Onboarding Framework

The skill implements a 13-screen archetype sequence based on the Mob recipe app's onboarding (the gold standard reference). The psychological sequence is:

1. **Hook** — Welcome + app preview showing the end state
2. **Goal elicitation** — "What are you trying to achieve?" (single-select, creates investment)
3. **Pain discovery** — "What prevents you?" (multi-select, surfaces frustrations)
4. **Social proof** —
```

</details>
