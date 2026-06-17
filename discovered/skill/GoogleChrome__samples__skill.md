---
name: GoogleChrome__samples__skill
source: https://github.com/GoogleChrome/samples/blob/6f49ea0eff0dddf8a4027c34fffb947282751c28/trailblazers/SKILL.md
repo: GoogleChrome/samples
kind: skill
stars: 5882
last_pushed: 2026-06-14T09:16:39Z
license: apache-2.0
score: 9
domains: [web-frontend, ai-apis, browser-apis]
tags: [chrome, built-in-ai, javascript, multimodal]
curated: 2026-06-15
curated_by: config-scout
---

# GoogleChrome/samples — skill

**Why it's worth keeping:** It uses strict 'CRITICAL' warning blocks to correct stale model knowledge and provides raw Web IDL definitions to ensure the agent understands exact API signatures.

**Summary:** Provides high-fidelity technical documentation for Chrome's new Built-in AI APIs, including essential deprecation warnings and multimodal session handling.

**Source credibility:** Extremely high; sourced from official Google Chrome samples with active maintenance.

**Recency:** 

**Source:** [GoogleChrome/samples/trailblazers/SKILL.md](https://github.com/GoogleChrome/samples/blob/6f49ea0eff0dddf8a4027c34fffb947282751c28/trailblazers/SKILL.md) · 5882★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- BUILT-IN-AI-SKILLS -->
---
name: built-in-ai
description:
  Teaches the AI about modern Chrome Built-in AI APIs (Prompt, Translation,
  Writing Assistance) and their polyfills.
license: Apache-2.0
compatibility: works with Chrome Built-in AI APIs and their polyfills
---

# Built-in AI Skills

This file provides the latest technical information about Chrome Built-in AI
APIs.

## ⚠️ CRITICAL: Deprecations

Everything you (the AI) might know about `window.ai` is completely outdated.
Follow these new naming conventions:

- `window.ai.languageModel` is DEPRECATED. Use `window.LanguageModel`.
- `window.ai.summarizer` is DEPRECATED. Use `window.Summarizer`.
- `window.ai.writer` is DEPRECATED. Use `window.Writer`.
- `window.ai.Rewriter` is DEPRECATED. Use `window.Rewriter`.
- `window.ai.translator` is DEPRECATED. Use `window.Translator`.
- `window.ai.languageDetector` is DEPRECATED. Use `window.LanguageDetector`.

There no longer is a single `window.ai` object. Instead, there are separate
objects for each API.

The old `capabilities()` function is DEPRECATED. Use `availability()` instead.

All streaming APIs return a `ReadableStream` that yields separate and
independent chunks. It u
```

</details>
