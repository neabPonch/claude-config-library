---
name: henry-md__intention-setting__claude
source: https://github.com/henry-md/intention-setting/blob/5ea04f5dbda13bdbd2ce2337266a50bf015fbb5e/.claude/CLAUDE.md
repo: henry-md/intention-setting
kind: claude-md
stars: 0
last_pushed: 2026-05-09T03:35:58Z
license: unknown
score: 8
domains: [web-extension, security, chrome-extension]
tags: [manifest-v3, firebase, architecture, guardrails]
curated: 2026-06-16
curated_by: config-scout
---

# henry-md/intention-setting — claude-md

**Why it's worth keeping:** The 'General Rules' prevent AI laziness and unnecessary migration overhead, while the technical section provides explicit constraints to avoid common MV3/CSP errors.

**Summary:** Establishes strict architectural guardrails for implementing Firebase OAuth within a Chrome Extension Manifest V3 environment.

**Source credibility:** A personal project with low visibility but highly specific technical constraints.

**Recency:** Highly relevant to modern Chrome Extension development standards (MV3).

**Source:** [henry-md/intention-setting/.claude/CLAUDE.md](https://github.com/henry-md/intention-setting/blob/5ea04f5dbda13bdbd2ce2337266a50bf015fbb5e/.claude/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# General Rules
- DO NOT create backwards compatability migrations in the project. Whiping the database is no bid deal right now — this is a personal project. We want to avoid bloat. Absolutely NO need for backwards compatability.
- Do not tell me to check something in my codebase without checking it yourself first. To restate, because this is important, DO NOT give me an answer telling me to verify X about the codebase — you have the code in front of you, verify yourself! You may tell me what you found afterwards.
- If the question is asking for clarification specifically, it is ok to answer very simply. However if the question is more in the spirit of trying to learn things (as opposed to asking clarification for something I think I already know), do not be afriad to add as much context as you would like. Feel free to give short and long answers when appropriate.

# Firebase OAuth Chrome Extension Architecture

**Important:** Chrome Extension Manifest V3 (MV3) imposes strict Content Security Policy (CSP) restrictions, which block inline scripts and remote script injection. This mean certain approaches and things, especially integrations with third party tools, have lots of depric
```

</details>
