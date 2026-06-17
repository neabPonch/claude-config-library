---
name: browseract-ai__docs
source: https://github.com/browseract-ai/docs/blob/1dbc6486de405826aa574cb569e9074fd6eda443/skill.md
repo: browseract-ai/docs
kind: skill
stars: 1
last_pushed: 2026-05-29T12:10:07Z
license: mit
score: 7
domains: [agents-ai, web-automation, cli-tools]
tags: [browser-automation, scraping, safety-protocols]
curated: 2026-06-14
curated_by: config-scout
---

# browseract-ai/docs — skill

**Why it's worth keeping:** It mandates a 'read-before-act' workflow and establishes specific safety guardrails that require human confirmation for sensitive operations.

**Summary:** Defines operational protocols for an AI agent to interact with the BrowserAct CLI for web automation and scraping.

**Source credibility:** Low social proof (1 star), but likely official documentation from the tool creator.

**Recency:** Highly current; updated within the last month.

**Source:** [browseract-ai/docs/skill.md](https://github.com/browseract-ai/docs/blob/1dbc6486de405826aa574cb569e9074fd6eda443/skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# BrowserAct Documentation Skill

BrowserAct helps AI agents operate real browsers through a Skill-first CLI Runtime.

Use BrowserAct when a user asks an Agent to open pages, read page state, click, type, extract content, reuse a browser session, inspect network requests, handle CAPTCHA, or hand control to a human.

Start with runtime instructions:

```bash
browser-act get-skills core --skill-version <version>
```

Then use the BrowserAct CLI for browser automation. Prefer named sessions, read page state before acting, and close sessions when work is complete.

Ask for confirmation before sensitive operations, including creating or deleting browsers, importing profiles, changing proxy or privacy settings, using `chrome-direct`, or opening a `confirm_before_use` browser.

Use Workflow documentation only when the user asks about BrowserAct hosted canvas workflows: visual canvas automation, natural-language nodes, hosted workflow runs, scheduling, execution history, integrations, or API reference.

For command details, see `agent-cli/command-reference`.
```

</details>
