---
name: understudy-ai__understudy__skill
source: https://github.com/understudy-ai/understudy/blob/f90f09fad6a476f3f2c8cb2689e76c72eb2c8a3c/skills/oracle/SKILL.md
repo: understudy-ai/understudy
kind: skill
stars: 435
last_pushed: 2026-06-14T10:02:46Z
license: mit
score: 8
domains: [cli-tools, agents-ai, workflow-optimization]
tags: [context-bundling, prompt-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# understudy-ai/understudy — skill

**Why it's worth keeping:** The 'Exhaustive prompt restoration pattern' and specific project briefing constraints are highly transferable mental models for effective LLM prompting.

**Summary:** Provides instructions for using the oracle CLI to bundle local file context into high-signal prompts for remote LLM sessions.

**Source credibility:** High; 435 stars and very recent maintenance activity.

**Recency:** Current, targeting modern high-context model workflows.

**Source:** [understudy-ai/understudy/skills/oracle/SKILL.md](https://github.com/understudy-ai/understudy/blob/f90f09fad6a476f3f2c8cb2689e76c72eb2c8a3c/skills/oracle/SKILL.md) · 435★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: oracle
description: Best practices for using the oracle CLI (prompt + file bundling, engines, sessions, and file attachment patterns).
homepage: https://askoracle.dev
metadata:
  {
    "understudy":
      {
        "emoji": "🧿",
        "requires": { "bins": ["oracle"] },
        "install":
          [
            {
              "id": "node",
              "kind": "node",
              "package": "@steipete/oracle",
              "bins": ["oracle"],
              "label": "Install oracle (node)",
            },
          ],
      },
  }
---

# oracle — best use

Oracle bundles your prompt + selected files into one “one-shot” request so another model can answer with real repo context (API or browser automation). Treat output as advisory: verify against code + tests.

## Main use case (browser, GPT‑5.2 Pro)

Default workflow here: `--engine browser` with GPT‑5.2 Pro in ChatGPT. This is the common “long think” path: ~10 minutes to ~1 hour is normal; expect a stored session you can reattach to.

Recommended defaults:

- Engine: browser (`--engine browser`)
- Model: GPT‑5.2 Pro (`--model gpt-5.2-pro` or `--model "5.2 Pro"`)

## Golden path

1. Pick a tight file set (fewest fi
```

</details>
