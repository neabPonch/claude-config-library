---
name: Vyro-ai__imagine-campaign-director
source: https://github.com/Vyro-ai/imagine-campaign-director/blob/f4a7db48167d1280a58ab06bd35392d1f769571f/skill.md
repo: Vyro-ai/imagine-campaign-director
kind: skill
stars: 2
last_pushed: 2026-05-06T17:40:38Z
license: other
score: 8
domains: [creative-production, agents-ai, automation]
tags: [video-generation, computer-use, workflow-orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# Vyro-ai/imagine-campaign-director — skill

**Why it's worth keeping:** Provides an excellent template for 'Capability Preflighting' (verifying computer use/browser access before proceeding) and strict tool-use hierarchy to prevent agent deviation.

**Summary:** Orchestrates complex video production by transitioning from high-level creative direction to automated browser execution. It uses a rigorous multi-stage pipeline involving treatments, specific tool routing, and quality gates.

**Source credibility:** Low star count, but the complexity of the logic suggests a highly specialized production tool.

**Recency:** Highly current; designed specifically for the 'Computer Use' capabilities era.

**Source:** [Vyro-ai/imagine-campaign-director/skill.md](https://github.com/Vyro-ai/imagine-campaign-director/blob/f4a7db48167d1280a58ab06bd35392d1f769571f/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# imagine-campaign-director for Imagine.Art

Use this skill when an agent needs to create a polished campaign video through Imagine.Art Workflows.

## Primary Job

Turn any reasonable campaign input into a complete Imagine.Art production workflow package:

- brief
- raw prompt
- style image
- product photo
- mood board
- reference images
- existing footage
- brand notes
- mixed assets

The output should follow `docs/PRODUCTION_STANDARD.md`.

## Required Default

Always plan generation through Imagine.Art Workflows unless the user explicitly asks for a different platform.

Use platform-neutral language only as secondary portability notes. Brand assets, product photos, mood boards, and style images are creative direction and continuity references; they should guide production choices and final lockup.

If Computer Use, browser automation, or desktop control is available, the agent should execute the workflow in Imagine.Art by default. Follow `docs/AUTOMATION_CONTRACT.md` and `prompts/imagineart_browser_operator.md`.

## Computer Use Execution Rule

For campaign-video requests, the first action is a Computer Use/browser automation capability preflight. This only verifies whether Imagi
```

</details>
