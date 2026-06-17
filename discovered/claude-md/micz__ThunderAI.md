---
name: micz__ThunderAI
source: https://github.com/micz/ThunderAI/blob/d0aec9b42ff0fa02f785963d9ae83804059b897e/CLAUDE.md
repo: micz/ThunderAI
kind: claude-md
stars: 310
last_pushed: 2026-06-14T21:23:10Z
license: gpl-3.0
score: 9
domains: [web-extension, javascript]
tags: [manifest-v2, zero-build, spec-driven]
curated: 2026-06-15
curated_by: config-scout
---

# micz/ThunderAI — claude-md

**Why it's worth keeping:** Uses negative constraints to prevent tool-chain hallucinations (like assuming npm/bundlers) and mandates a spec-first development loop.

**Summary:** Provides strict architectural constraints for a zero-build WebExtension and defines specific workflows for localization and settings.

**Source credibility:** High; a popular, actively maintained open-source project with 310 stars.

**Recency:** Extremely current; updated within the last month.

**Source:** [micz/ThunderAI/CLAUDE.md](https://github.com/micz/ThunderAI/blob/d0aec9b42ff0fa02f785963d9ae83804059b897e/CLAUDE.md) · 310★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ThunderAI - Claude Code Guide

## Project Overview
ThunderAI is a **Thunderbird WebExtension (Manifest V2)** that integrates multiple AI providers (ChatGPT Web, OpenAI API, Google Gemini, Claude/Anthropic, Ollama, and OpenAI-compatible APIs) directly into the Thunderbird email client.

- **Extension ID:** `thunderai@micz.it`
- **Min Thunderbird:** 140.0+
- **Language:** Plain ES6+ JavaScript modules — no build tools, no transpilation, no npm
- **License:** GPLv3

## Key Rules

1. **Localization:** Modify ONLY `_locales/en/messages.json`. All other locale files are managed via Weblate — never touch them.
2. **No build system:** There is no bundler, compiler, or package manager. All JS files are plain ES6 modules loaded directly by the browser engine.
3. **Module imports:** Use relative paths with `.js` extension (e.g., `import { foo } from '../js/mzta-utils.js'`).
4. **Placeholder format:** Placeholders in prompt text use the `{%placeholder_id%}` syntax (e.g., `{%mail_text_body_or_selected%}`).
5. **No test suite:** There is no automated test framework. Testing is done manually in Thunderbird.
6. **Settings defaults:** All new preferences must be added to `options/mzta-options-def
```

</details>
