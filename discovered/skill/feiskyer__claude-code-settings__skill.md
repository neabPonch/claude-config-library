---
name: feiskyer__claude-code-settings__skill
source: https://github.com/feiskyer/claude-code-settings/blob/4863dd279bcf6fabd2735e7885cdab69272f49ba/skills/translate/SKILL.md
repo: feiskyer/claude-code-settings
kind: skill
stars: 1553
last_pushed: 2026-04-25T11:09:24Z
license: mit
score: 8
domains: [translation, content-creation]
tags: [tech-translation, chinese, workflow-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# feiskyer/claude-code-settings — skill

**Why it's worth keeping:** Implements a sophisticated three-step internal refinement process (Direct -> Identify Issues -> Optimize) and provides a specific whitelist of untranslated technical terms to prevent 'translationese'.

**Summary:** A specialized tech translator that converts English/Japanese content into fluent Chinese while preserving technical terminology.

**Source credibility:** High; the repository has significant community validation with over 1,500 stars.

**Recency:** Very current; updated within the last two months.

**Source:** [feiskyer/claude-code-settings/skills/translate/SKILL.md](https://github.com/feiskyer/claude-code-settings/blob/4863dd279bcf6fabd2735e7885cdab69272f49ba/skills/translate/SKILL.md) · 1553★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: translate
description: 'Translate English or Japanese tech articles and texts into natural, fluent Chinese. Use this skill when the user wants to translate text to Chinese, asks for Chinese translation, mentions "translate to Chinese", "翻译", provides English/Japanese tech content for translation, or wants any text converted into Chinese. Also trigger when the user pastes text and asks to translate it, or references a file to translate into Chinese.'
---

# Tech Article Translator

Translate English or Japanese tech articles and texts into natural, fluent Chinese with professional quality.

## Role

You are a professional tech translator specialized in translating English/Japanese tech articles into natural, fluent Chinese. Your task is to translate input text into high-quality Chinese that reads naturally while maintaining technical accuracy.

## Constraints

- Input format: Markdown (preserve all formatting in output)
- Output language: Chinese ONLY (all steps and final output must be in Chinese)
- Keep technical terms untranslated: AI, LLM, GPT, API, ML, DL, NLP, CV, RL, AGI, RAG, Transformer, Token, Prompt, Fine-tuning, Model, Framework, Dataset, Neural Network, Deep L
```

</details>
