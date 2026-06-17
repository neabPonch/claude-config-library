---
name: OneWave-AI__claude-skills__skill
source: https://github.com/OneWave-AI/claude-skills/blob/a8cde4bd44169c13212b854738ba9b968d6f0b2e/animate/SKILL.md
repo: OneWave-AI/claude-skills
kind: skill
stars: 185
last_pushed: 2026-06-08T01:30:35Z
license: mit
score: 9
domains: [web-frontend, creative-coding, cli-tools]
tags: [animation, react, framer-motion, visuals]
curated: 2026-06-15
curated_by: config-scout
---

# OneWave-AI/claude-skills — skill

**Why it's worth keeping:** The skill provides a controlled vocabulary of scene transitions and element animations, which prevents the LLM from hallucinating poor motion patterns. It also uses a structured scaffolding workflow that ensures high-quality, responsive outputs through specific CSS/component standards.

**Summary:** Transforms natural language descriptions into standalone Vite + React animation projects using Framer Motion, p5.js, or Three.js.

**Source credibility:** High; 185 stars and active maintenance by OneWave AI suggest a production-ready toolset.

**Recency:** 

**Source:** [OneWave-AI/claude-skills/animate/SKILL.md](https://github.com/OneWave-AI/claude-skills/blob/a8cde4bd44169c13212b854738ba9b968d6f0b2e/animate/SKILL.md) · 185★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: animate
description: Generate animated videos and motion graphics from natural language descriptions. Creates a standalone Vite + React project with Framer Motion scenes that auto-play in the browser. Use when the user wants to create animations, motion graphics, video intros, animated presentations, or product demos.
argument-hint: [description of the animation you want]
allowed-tools: Read, Write, Edit, Bash, Glob, Grep, WebFetch, WebSearch
---

# Animation Generator

Create animated videos and motion graphics from a natural language description. Outputs a standalone Vite + React + Framer Motion project that plays in the browser.

## Workflow

### Step 1: Parse the Request

Break the user's description into a scene plan:
- **3-7 scenes**, each 3-5 seconds long
- Identify the story arc: hero/intro, problem, solution, features, CTA/outro
- Pick a color palette and typography that fits the brand/mood
- Use `$ARGUMENTS` for the user's animation description

### Step 2: Choose the Animation Stack

Auto-detect the best approach based on the request:

| Request Type | Stack | When to Use |
|---|---|---|
| Product intro, presentation, marketing | **Framer Motion** (default) | S
```

</details>
