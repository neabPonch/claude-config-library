---
name: NoxDevelopment__unitygen
source: https://github.com/NoxDevelopment/unitygen/blob/675bba41d648bade9fb19164dbdf85b48b68a036/CLAUDE.md
repo: NoxDevelopment/unitygen
kind: claude-md
stars: 0
last_pushed: 2026-05-29T15:20:51Z
license: mit
score: 8
domains: [game-development, unity-engine, ai-agents]
tags: [unity, game-dev, orchestration, architectural-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# NoxDevelopment/unitygen — claude-md

**Why it's worth keeping:** The 'Design rules' section provides exceptional meta-instructions: avoiding handholding to save context, requiring explanations of 'why' for engine quirks, and prioritizing data-driven workflows (ScriptableObjects/Addressables) over hardcoded logic.

**Summary:** Provides a dual-agent architecture consisting of an orchestrator for high-level planning and a task executor for specific C# implementation. It focuses on bridging the gap between high-level game design and low-level Unity engine mechanics.

**Source credibility:** Low star count suggests a niche tool, but the high technical density indicates deep domain expertise in Unity development.

**Recency:** Very current; pushed within the last month during the rise of Claude Code-style workflows.

**Source:** [NoxDevelopment/unitygen/CLAUDE.md](https://github.com/NoxDevelopment/unitygen/blob/675bba41d648bade9fb19164dbdf85b48b68a036/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
We develop agents and skills here. They are then used in another folder for Unity game development with Claude Code.

## Layout

Source at the repo root:
- `skills/unitygen/` — orchestrator: SKILL.md + Unity-specific primers (MonoBehaviour, ScriptableObject, Addressables, Input System, URP/HDRP, UIToolkit, Packages, DOTS, C# rules)
- `skills/unity-task/` — task executor: SKILL.md + C# reference + asmdef + Test Framework + headless build + play-mode QA
- `publish.sh` — copy into a target Unity project's `.claude/skills/`
- Pair with `gamegen` for engine-agnostic personas, commands, templates, and rules.

## Skills

- unitygen — orchestrator + scaffold + decomposer + asset planning + asset generation (main thread)
- unity-task — task execution + C# docs + Play Mode harness + screenshot capture + visual QA (context: fork)

## Design rules

- Don't handhold. The agent is a capable LLM; obvious guidance pollutes context.
- Engine-specific content only. Engine-agnostic material (design docs, retros, accessibility) belongs in `gamegen`.
- Every file earns its existence by changing a decision. "Be careful with null" is not a file.
- Prefer ScriptableObject + data assets over code branches.
```

</details>
